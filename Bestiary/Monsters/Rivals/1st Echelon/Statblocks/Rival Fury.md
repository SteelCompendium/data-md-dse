---
agility: 1
ancestry:
- Humanoid
- Rival
ev: '16'
file_basename: Rival Fury
file_dpath: Monsters/Rivals/1st Echelon/Statblocks
free_strike: 5
intuition: 0
item_id: rival-fury
item_index: 08
item_name: Rival Fury
level: 2
might: 2
presence: 0
reason: 0
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:rival-fury
scdc:
- 1.1.1:2:08
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 3
stamina: '100'
type: monster
---

```ds-statblock
name: Rival Fury
level: 2
roles:
  - Elite Brute
ancestry:
  - Humanoid
  - Rival
ev: "16"
stamina: "100"
speed: 5
size: 1M
stability: 3
free_strike: 5
might: 2
agility: 1
reason: 0
intuition: 0
presence: 0
traits:
  - name: Overwhelm
    effects:
      - effect: Once per turn, when the fury force moves a creature or object, or shifts
          adjacent to a creature or object, they can make a free strike against
          that creature or object.
  - name: Rivalry
    effects:
      - effect: At the start of an encounter, the fury chooses one creature within their
          line of effect. Both the fury and the creature can add a d3 roll to
          power rolls they make against each other.
abilities:
  - name: Brutal Impact
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
        t1: 7 damage; push 1
        t2: 11 damage; push 2
        t3: 14 damage; push 3
      - effect: Each target who has M < 1 is slowed (save ends).
        cost: 2 Malice
  - name: Let's Tussle
    cost: 2 Malice
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature
    effects:
      - roll: Power Roll + 2
        t1: 8 damage; M < 0 grabbed
        t2: 13 damage; M < 1 grabbed
        t3: 16 damage; M < 2 grabbed
      - effect: The target must be the fury's size or smaller. While the target is
          grabbed this way, the fury gains an edge on strikes against them.
        name: Effect
```