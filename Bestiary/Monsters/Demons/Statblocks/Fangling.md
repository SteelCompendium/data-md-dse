---
agility: 2
ancestry:
- Abyssal
- Demon
ev: '6'
file_basename: Fangling
file_dpath: Monsters/Demons/Statblocks
free_strike: 2
intuition: 0
item_id: fangling
item_index: '262'
item_name: Fangling
level: 4
might: 3
presence: 0
reason: 0
roles:
- Horde Harrier
scc:
- mcdm.monsters.v1:monster:fangling
scdc:
- 1.1.1:2:262
size: 1L
source: mcdm.monsters.v1
speed: 8
stability: 0
stamina: '30'
type: monster
---

```ds-statblock
name: Fangling
level: 4
roles:
  - Horde Harrier
ancestry:
  - Abyssal
  - Demon
ev: "6"
stamina: "30"
weaknesses:
  - Holy 5
speed: 8
size: 1L
stability: 0
free_strike: 2
might: 3
agility: 2
reason: 0
intuition: 0
presence: 0
traits:
  - name: Made of Teeth
    effects:
      - effect: Whenever an adjacent enemy grabs the fangling or uses a melee ability
          against the fangling, they take 2 damage.
  - name: Lethe
    effects:
      - effect: While the fangling is winded, they gain an edge on strikes, and any
          strike made against them gains an edge.
  - name: Soulsight
    effects:
      - effect: Any creature within 2 squares of the fangling can't be hidden from them
abilities:
  - name: Tooth! Tusk! Claw!
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        t1: 5 damage
        t2: 7 damage
        t3: 9 damage
      - effect: Each enemy adjacent to the fangling takes 2 damage.
  - name: Tumbling Gore
    cost: 2 Malice
    keywords:
      - Area
      - Weapon
    type: Maneuver
    distance: 8 x 3 line within 1
    target: Each enemy in the area
    effects:
      - effect: e 8 x 3 line within 1 x Each enemy in the area
      - roll: Power Roll + 2
        t1: 2 damage; pull 1; A < 1 bleeding (save ends)
        t2: 3 damage; pull 1; A < 2 bleeding (save ends)
        t3: 4 damage; pull 1; A < 3 bleeding (save ends)
```