---
agility: 2
ancestry:
- Humanoid
- Time Raider
ev: '10'
file_basename: Time Raider Helix
file_dpath: Monsters/Time Raiders/Statblocks
free_strike: 5
intuition: 2
item_id: time-raider-helix
item_index: '145'
item_name: Time Raider Helix
level: 3
might: 0
presence: 2
reason: 2
roles:
- Platoon Controller
scc:
- mcdm.monsters.v1:monster:time-raider-helix
scdc:
- 1.1.1:2:145
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '40'
type: monster
---

~~~ds-statblock
type: statblock
name: Time Raider Helix
level: 3
roles:
  - Platoon Controller
ancestry:
  - Humanoid
  - Time Raider
ev: "10"
stamina: "40"
immunities:
  - Psychic 3
speed: 5
movement: Fly
size: 1M
stability: 0
free_strike: 5
might: 0
agility: 2
reason: 2
intuition: 2
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Blaster Volley
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Psionic
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        tier1: 6 corruption damage; push 2
        tier2: 8 corruption damage; push 4
        tier3: 11 corruption damage; push 6, prone
  - type: feature
    feature_type: ability
    name: Kinetic Lane
    icon: 🔳
    keywords:
      - Area
      - Psionic
      - Ranged
    usage: Maneuver
    distance: 4 x 2 line within 10
    target: Special
    effects:
      - name: Effect
        effect: The area is a psionically charged treadmill that pushes creatures and
          objects at high speed in one direction of the helix's choice. Any
          creature who enters the area or starts their turn there slides 3
          squares toward the end of the area in the chosen direction. Each enemy
          in the area when it first appears takes 3 damage before they slide
      - cost: 3 Malice
        effect: The helix creates a second kinetic lane.
  - type: feature
    feature_type: trait
    name: Foresight
    icon: ⭐️
    effects:
      - effect: The helix doesn't take a bane on strikes against creatures with
          concealment.
~~~