---
agility: 2
ancestry:
- Humanoid
- Orc
ev: '6'
file_basename: Orc Chainlock
file_dpath: Monsters/Orcs/Statblocks
free_strike: 3
intuition: 0
item_id: orc-chainlock
item_index: '125'
item_name: Orc Chainlock
level: 1
might: 2
presence: 0
reason: 1
roles:
- Platoon Hexer
scc:
- mcdm.monsters.v1:monster:orc-chainlock
scdc:
- 1.1.1:2:125
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '20'
type: monster
---

~~~ds-statblock
name: Orc Chainlock
level: 1
roles:
  - Platoon Hexer
ancestry:
  - Humanoid
  - Orc
ev: "6"
stamina: "20"
speed: 5
size: 1L
stability: 2
free_strike: 3
might: 2
agility: 2
reason: 1
intuition: 0
presence: 0
traits:
  - name: Chain Link
    effects:
      - effect: Whenever the chainlock is force moved by a creature's melee ability, the
          creature is pulled the same distance toward the chainlock after the
          forced movement is resolved.
  - name: Relentless
    effects:
      - effect: If the chainlock is reduced to 0 Stamina, they can make a free strike
          before dying. If the target of the free strike is reduced to 0
          Stamina, the chainlock is reduced to 1 Stamina instead.
abilities:
  - name: Hook and Chain
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 3
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 5 damage; pull 1; M < 0 the target is hooked (save ends)
        t2: 7 damage; pull 2; M < 1 the target is hooked (save ends)
        t3: 9 damage; pull 3; M < 2 the target is hooked (save ends)
      - effect: A hooked target can't move more than 3 squares away from the chainlock's
          position when this ability is used.
        name: Effect
  - name: Heavy Crossbolt
    icon: 🏹
    cost: 3 Malice
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 5
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 5 damage; A < 0 slowed (save ends)
        t2: 7 damage; A < 1 slowed (save ends)
        t3: 9 damage; prone; A < 2 slowed (save ends)
~~~