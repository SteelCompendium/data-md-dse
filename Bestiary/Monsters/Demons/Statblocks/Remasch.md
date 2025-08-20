---
agility: 2
ancestry:
- Abyssal
- Demon
ev: '4'
file_basename: Remasch
file_dpath: Monsters/Demons/Statblocks
free_strike: 3
intuition: 0
item_id: remasch
item_index: '279'
item_name: Remasch
level: 2
might: 0
presence: 2
reason: 0
roles:
- Horde Ambusher
scc:
- mcdm.monsters.v1:monster:remasch
scdc:
- 1.1.1:2:279
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '20'
type: monster
---

```ds-statblock
name: Remasch
level: 2
roles:
  - Horde Ambusher
ancestry:
  - Abyssal
  - Demon
ev: "4"
stamina: "20"
weaknesses:
  - Holy 3
speed: 5
movement: Teleport
size: 1S
stability: 0
free_strike: 3
might: 0
agility: 2
reason: 0
intuition: 0
presence: 2
traits:
  - name: Lethe
    effects:
      - effect: While the remasch is winded, they gain an edge on strikes, and any
          strike made against them gains an edge.
  - name: Soulsight
    effects:
      - effect: Any creature within 2 squares of the remasch can't be hidden from them.
abilities:
  - name: Abyssal Strike
    cost: Signature Ability
    keywords:
      - Magic
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 5 damage; the remasch can teleport up to 2 squares
        t2: 6 damage; the remasch can teleport up to 3 squares
        t3: 8 damage; the remasch can teleport up to 5 squares
      - effect: The remasch takes an adjacent creature with them when they teleport. The
          creature appears in an unoccupied space adjacent to the remasch's
          destination.
        cost: 5 Malice
  - name: Grasping Shadow
    cost: 3 Malice
    keywords:
      - Magic
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The remasch can teleport up to 2 squares and uses Abyssal Strike.
```