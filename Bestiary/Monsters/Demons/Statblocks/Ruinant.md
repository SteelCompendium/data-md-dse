---
agility: 2
ancestry:
- Abyssal
- Demon
ev: '3'
file_basename: Ruinant
file_dpath: Monsters/Demons/Statblocks
free_strike: 1
intuition: 0
item_id: ruinant
item_index: '285'
item_name: Ruinant
level: 1
might: 0
presence: 1
reason: 0
roles:
- Horde Harrier
scc:
- mcdm.monsters.v1:monster:ruinant
scdc:
- 1.1.1:2:285
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '15'
type: monster
---

```ds-statblock
name: Ruinant
level: 1
roles:
  - Horde Harrier
ancestry:
  - Abyssal
  - Demon
ev: "3"
stamina: "15"
weaknesses:
  - Holy 3
speed: 6
size: 1M
stability: 0
free_strike: 1
might: 0
agility: 2
reason: 0
intuition: 0
presence: 1
traits:
  - name: Lethe
    effects:
      - effect: While the ruinant is winded, they gain an edge on strikes, and any
          strike made against them gains an edge.
  - name: Soulsight
    effects:
      - effect: Any creature within 2 squares of the ruinant can't be hidden from them.
abilities:
  - name: Bloodletting Claws
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
        t1: 3 damage
        t2: 4 damage
        t3: 5 damage; M < 2 bleeding (save ends)
  - name: Salt Wounds
    icon: 🏹
    cost: 3 Malice
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Maneuver
    distance: Ranged 10
    target: Three creatures
    effects:
      - name: Special
        effect: Each target must be at less than full Stamina.
      - roll: Power Roll + 2
        t1: 1 corruption damage
        t2: 2 corruption damage
        t3: 3 corruption damage
```