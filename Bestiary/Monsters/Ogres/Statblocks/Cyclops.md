---
agility: -1
ancestry:
- Giant
- Ogre
ev: 12 for four minions
file_basename: Cyclops
file_dpath: Monsters/Ogres/Statblocks
free_strike: 4
intuition: 3
item_id: cyclops
item_index: '05'
item_name: Cyclops
level: 10
might: 5
presence: -1
reason: -1
roles:
- Minion Controller
scc:
- mcdm.monsters.v1:monster:cyclops
scdc:
- 1.1.1:2:05
size: '3'
source: mcdm.monsters.v1
speed: 6
stability: 5
stamina: '14'
type: monster
---

~~~ds-statblock
type: statblock
name: Cyclops
level: 10
roles:
  - Minion Controller
ancestry:
  - Giant
  - Ogre
ev: 12 for four minions
stamina: "14"
speed: 6
size: "3"
stability: 5
free_strike: 4
with_captain: +4 bonus to speed
might: 5
agility: -1
reason: -1
intuition: 3
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Wild Slam
    icon: ❇️
    ability_type: Signature Ability
    keywords:
      - Area
      - Weapon
    usage: Main action
    distance: 1 burst
    target: Each enemy and object in the area
    effects:
      - roll: Power Roll + 5
        tier1: 3 damage; A < 3 3 damage
        tier2: 6 damage; push 3; A < 4 4 damage
        tier3: 7 damage; prone; A < 5 5 damage and restrained (save ends)
      - name: Effect
        effect: The cyclops automatically treats their initial power roll as a 17. They
          can still roll to determine if they score a critical hit.
  - type: feature
    feature_type: trait
    name: Limited Vision
    icon: ⭐️
    effects:
      - effect: The cyclops has line of effect only within 3 squares. Whenever the
          cyclops takes damage from a ranged ability, they can move up to 3
          squares toward the source of the damage.
~~~