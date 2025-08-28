---
agility: 3
ancestry:
- Humanoid
- Rival
ev: '40'
file_basename: Rival Fury
file_dpath: Monsters/Rivals/3rd Echelon/Statblocks
free_strike: 9
intuition: 1
item_id: rival-fury
item_index: '22'
item_name: Rival Fury
level: 8
might: 4
presence: 2
reason: 0
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:rival-fury
scdc:
- 1.1.1:2:22
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 3
stamina: '220'
type: monster
---

~~~ds-statblock
name: Rival Fury
level: 8
roles:
  - Elite Brute
ancestry:
  - Humanoid
  - Rival
ev: "40"
stamina: "220"
speed: 5
size: 1M
stability: 3
free_strike: 9
might: 4
agility: 3
reason: 0
intuition: 1
presence: 2
traits:
  - name: Rout
    effects:
      - effect: Once per turn, when the fury force moves a creature or object, or shifts
          adjacent to a creature or object, they can use a signature ability
          that gains an edge against that creature or object.
  - name: Rivalry
    effects:
      - effect: At the start of an encounter, the fury chooses one creature within their
          line of effect. Both the fury and the creature can add a d3 roll to
          power rolls they make against each other.
abilities:
  - name: Bonebreaker
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
      - roll: Power Roll + 4
        t1: 13 damage; push 3
        t2: 18 damage; push 4
        t3: 22 damage; push 5
      - effect: Each target who has M < 3 is bleeding and slowed (save ends).
        cost: 3 Malice
  - name: Steelfist
    icon: 🗡
    cost: 3 Malice
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature
    effects:
      - roll: Power Roll + 4
        t1: 15 damage; M < 3 grabbed
        t2: 21 damage; M < 4 grabbed
        t3: 26 damage; M < 5 grabbed
      - effect: The target must be the fury's size or smaller. While the target is
          grabbed this way, the fury and their allies have a double edge on
          strikes against them.
        name: Effect
~~~