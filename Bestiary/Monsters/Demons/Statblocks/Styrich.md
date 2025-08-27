---
agility: 4
ancestry:
- Abyssal
- Demon
ev: '10'
file_basename: Styrich
file_dpath: Monsters/Demons/Statblocks
free_strike: 3
intuition: 2
item_id: styrich
item_index: '260'
item_name: Styrich
level: 8
might: 2
presence: 0
reason: 0
roles:
- Horde Hexer
scc:
- mcdm.monsters.v1:monster:styrich
scdc:
- 1.1.1:2:260
size: 1L
source: mcdm.monsters.v1
speed: 6
stability: 1
stamina: '45'
type: monster
---

```ds-statblock
name: Styrich
level: 8
roles:
  - Horde Hexer
ancestry:
  - Abyssal
  - Demon
ev: "10"
stamina: "45"
weaknesses:
  - Holy 5
speed: 6
size: 1L
stability: 1
free_strike: 3
might: 2
agility: 4
reason: 0
intuition: 2
presence: 0
traits:
  - name: Lethe
    effects:
      - effect: While the styrich is winded, they gain an edge on strikes, and any
          strike made against them gains an edge.
  - name: Soulsight
    effects:
      - effect: Any creature within 2 squares of the styrich can't be hidden from them.
abilities:
  - name: Hair Whip
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 4
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        t1: 7 damage; pull 1
        t2: 10 damage; pull 2, grabbed
        t3: 12 damage; pull 3, grabbed
      - effect: Any target restrained by the styrich's Tangled Nest ability can be
          pulled the distance determined by the power roll.
        name: Effect
  - name: Tangled Nest
    icon: ❇️
    cost: 5 Malice
    keywords:
      - Area
    type: Maneuver
    distance: 4 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        t1: A < 2 slowed (save ends)
        t2: Slowed (EoT) or A < 3 3 damage and restrained (EoT)
        t3: Restrained (EoT) or A < 4 3 damage and restrained (save ends)
```