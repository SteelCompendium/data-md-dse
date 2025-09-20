---
agility: 2
ancestry:
- Abyssal
- Gnoll
ev: '4'
file_basename: Gnoll Abyssal Archer
file_dpath: Monsters/Gnolls/Statblocks
free_strike: 3
intuition: 0
item_id: gnoll-abyssal-archer
item_index: '35'
item_name: Gnoll Abyssal Archer
level: 2
might: 0
presence: -1
reason: 1
roles:
- Horde Artillery
scc:
- mcdm.monsters.v1:monster:gnoll-abyssal-archer
scdc:
- 1.1.1:2:35
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '15'
type: monster
---

~~~ds-statblock
type: statblock
name: Gnoll Abyssal Archer
level: 2
roles:
  - Horde Artillery
ancestry:
  - Abyssal
  - Gnoll
ev: "4"
stamina: "15"
speed: 5
size: 1M
stability: 1
free_strike: 3
might: 0
agility: 2
reason: 1
intuition: 0
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Dark Longbow
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 5 corruption damage
        tier2: 6 corruption damage
        tier3: 8 corruption damage; M < 2 slowed (save ends)
      - name: Effect
        effect: This ability gains an edge against any target not at full Stamina.
  - type: feature
    feature_type: ability
    name: Archer's Cackletongue
    icon: ❇️
    cost: 2 Malice
    keywords:
      - Area
    usage: Maneuver
    distance: 2 burst
    target: Self and each ally in the area
    effects:
      - name: Effect
        effect: Until the end of their next turn, each target gains an edge on their
          next strike. If any target hasn't used their own Cackletongue maneuver
          on this turn, they can use it immediately at no cost.
  - type: feature
    feature_type: trait
    name: Distant Death Frenzy
    icon: ⭐️
    effects:
      - effect: Whenever a non-minion ally within 5 squares of the abyssal archer is
          reduced to 0 Stamina, the abyssal archer can make a ranged free
          strike.
  - type: feature
    feature_type: trait
    name: Bloodscent
    icon: ⭐️
    effects:
      - effect: The abyssal archer doesn't need line of effect to use their abilities
          against any creature who isn't at full Stamina, as long as a size 1
          opening exists between the archer and the target.
~~~