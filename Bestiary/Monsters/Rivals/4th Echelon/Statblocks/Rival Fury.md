---
agility: 4
ancestry:
- Humanoid
- Rival
ev: '48'
file_basename: Rival Fury
file_dpath: Monsters/Rivals/4th Echelon/Statblocks
free_strike: 10
intuition: 2
item_id: rival-fury
item_index: '29'
item_name: Rival Fury
level: 10
might: 5
presence: 3
reason: 0
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:rival-fury
scdc:
- 1.1.1:2:29
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 3
stamina: '260'
type: monster
---

```ds-statblock
name: Rival Fury
level: 10
roles:
  - Elite Brute
ancestry:
  - Humanoid
  - Rival
ev: "48"
stamina: "260"
speed: 5
size: 1M
stability: 3
free_strike: 10
might: 5
agility: 4
reason: 0
intuition: 2
presence: 3
traits:
  - name: Devastate
    effects:
      - effect: Once per turn, when the fury force moves a creature or object, or shifts
          adjacent to a creature or object, they can use a signature ability
          against that creature or object that has a double edge.
  - name: Rivalry
    effects:
      - effect: At the start of an encounter, the fury chooses one creature within their
          line of effect. Both the fury and the creature can add a d3 roll to
          power rolls they make against each other.
abilities:
  - name: Seismic Crush
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 5
        t1: 15 damage; push 4
        t2: 21 damage; push 5
        t3: 25 damage; push 6
      - effect: Each target who has M < 4 is bleeding and slowed (save ends).
        cost: 2 Malice
  - name: Death Grip
    cost: 4 Malice
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature
    effects:
      - roll: Power Roll + 5
        t1: 15 damage; M < 3 grabbed
        t2: 21 damage; M < 4 grabbed
        t3: 25 damage; M < 5 grabbed
      - effect: The target must be the fury's size or smaller. While the target is
          grabbed this way, the fury and their allies have a double edge on
          strikes against them.
```