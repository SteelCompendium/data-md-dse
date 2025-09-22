---
agility: 2
ancestry:
- Humanoid
- Radenwight
ev: '6'
file_basename: Radenwight Ratcrobat
file_dpath: Monsters/Radenwights/Statblocks
free_strike: 3
intuition: 0
item_id: radenwight-ratcrobat
item_index: '152'
item_name: Radenwight Ratcrobat
level: 1
might: -1
presence: 1
reason: 0
roles:
- Platoon Harrier
scc:
- mcdm.monsters.v1:monster:radenwight-ratcrobat
scdc:
- 1.1.1:2:152
size: 1S
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '30'
type: monster
---

~~~ds-statblock
type: statblock
name: Radenwight Ratcrobat
level: 1
roles:
  - Platoon Harrier
ancestry:
  - Humanoid
  - Radenwight
ev: "6"
stamina: "30"
speed: 7
movement: Climb
size: 1S
stability: 0
free_strike: 3
might: -1
agility: 2
reason: 0
intuition: 0
presence: 1
features:
  - type: feature
    feature_type: ability
    name: En Garde
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        tier1: 4 damage
        tier2: 6 damage
        tier3: 8 damage
      - name: Effect
        effect: The ratcrobat shifts up to 2 squares after striking the first target,
          then can shift 1 square after striking the second target.
  - type: feature
    feature_type: ability
    name: Over Here, Thanks
    icon: 🗡
    keywords:
      - Melee
    usage: Maneuver
    distance: Melee 1
    target: One enemy
    effects:
      - name: Effect
        effect: The ratcrobat slides the target up to 3 squares, then can shift into any
          square the target left.
  - type: feature
    feature_type: ability
    name: Ready Rodent
    icon: ❗️
    keywords:
      - Melee
      - Weapon
    usage: Triggered action
    distance: Melee 1
    target: One creature
    trigger: An ally deals damage to the target.
    effects:
      - name: Effect
        effect: The ratcrobat makes a free strike against the target.
  - type: feature
    feature_type: trait
    name: Gymratstics
    icon: ⭐️
    effects:
      - effect: The ratcrobat gains an edge on strikes against larger creatures.
~~~