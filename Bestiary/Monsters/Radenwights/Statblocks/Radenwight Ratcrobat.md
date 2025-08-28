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
traits:
  - name: Gymratstics
    effects:
      - effect: The ratcrobat gains an edge on strikes against larger creatures.
abilities:
  - name: En Garde
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        t1: 4 damage
        t2: 6 damage
        t3: 8 damage
      - effect: The ratcrobat shifts up to 2 squares after striking the first target,
          then can shift 1 square after striking the second target.
        name: Effect
  - name: Over Here, Thanks
    icon: 🗡
    keywords:
      - Melee
    type: Maneuver
    distance: Melee 1
    target: One enemy
    effects:
      - effect: The ratcrobat slides the target up to 3 squares, then can shift into any
          square the target left
        name: Effect
  - name: Ready Rodent
    icon: ❗️
    keywords:
      - Melee
      - Weapon
    type: Triggered action
    distance: Melee 1
    target: One creature
    trigger: An ally deals damage to the target.
    effects:
      - effect: The ratcrobat makes a free strike against the target.
        name: Effect
~~~