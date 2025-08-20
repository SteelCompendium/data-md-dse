---
agility: 2
ancestry:
- Abyssal
- Demon
ev: 6 for four minions
file_basename: Grulqin
file_dpath: Monsters/Demons/Statblocks
free_strike: 3
intuition: -1
item_id: grulqin
item_index: '269'
item_name: Grulqin
level: 4
might: 3
presence: -1
reason: -1
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster:grulqin
scdc:
- 1.1.1:2:269
size: 1L
source: mcdm.monsters.v1
speed: 8
stability: 1
stamina: '9'
type: monster
---

```ds-statblock
name: Grulqin
level: 4
roles:
  - Minion Brute
ancestry:
  - Abyssal
  - Demon
ev: 6 for four minions
stamina: "9"
weaknesses:
  - Holy 5
speed: 8
size: 1L
stability: 1
free_strike: 3
with_captain: +2 damage bonus to strikes
might: 3
agility: 2
reason: -1
intuition: -1
presence: -1
traits:
  - name: Soulsight
    effects:
      - effect: Any creature within 2 squares of the grulqin can't be hidden from them.
abilities:
  - name: Spinning Bone Blade
    cost: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 3
        t1: 3 damage
        t2: 5 damage
        t3: 7 damage
      - effect: The grulqin gains an edge on this ability if they previously moved 3 or
          more squares in a straight line on their turn.
```