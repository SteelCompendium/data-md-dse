---
agility: 2
ancestry:
- Humanoid
- Radenwight
ev: 3 for 4 minions
file_basename: Radenwight Swiftpaw
file_dpath: Monsters/Radenwights/Statblocks
free_strike: 1
intuition: 0
item_id: radenwight-swiftpaw
item_index: '156'
item_name: Radenwight Swiftpaw
level: 1
might: 0
presence: -1
reason: 1
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster:radenwight-swiftpaw
scdc:
- 1.1.1:2:156
size: 1S
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '4'
type: monster
---

~~~ds-statblock
type: statblock
name: Radenwight Swiftpaw
level: 1
roles:
  - Minion Harrier
ancestry:
  - Humanoid
  - Radenwight
ev: 3 for 4 minions
stamina: "4"
speed: 7
movement: Climb
size: 1S
stability: 0
free_strike: 1
with_captain: Gain an edge on strikes
might: 0
agility: 2
reason: 1
intuition: 0
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Rapier Flunge
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 1 damage; slide 1, the swiftpaw can shift 1 square
        tier2: 2 damage; slide 2, the swiftpaw shifts up to 2 squares
        tier3: 3 damage; slide 3, the swiftpaw shifts up to 3 squares
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
        effect: The swiftpaw makes a free strike against the target.
~~~