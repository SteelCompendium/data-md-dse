---
agility: 0
ancestry:
- Abyssal
- Demon
ev: 3 for four minions
file_basename: Ensnarer
file_dpath: Monsters/Demons/Statblocks
free_strike: 2
intuition: -1
item_id: ensnarer
item_index: '257'
item_name: Ensnarer
level: 1
might: 2
presence: -1
reason: -1
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster:ensnarer
scdc:
- 1.1.1:2:257
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '5'
type: monster
---

```ds-statblock
name: Ensnarer
level: 1
roles:
  - Minion Brute
ancestry:
  - Abyssal
  - Demon
ev: 3 for four minions
stamina: "5"
weaknesses:
  - Holy 3
speed: 5
size: 1M
stability: 0
free_strike: 2
with_captain: +2 bonus to melee distance
might: 2
agility: 0
reason: -1
intuition: -1
presence: -1
traits:
  - name: Soulsight
    effects:
      - effect: Any creature within 2 squares of the ensnarer can't be hidden from them.
abilities:
  - name: Barbed Tongues
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 3
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        t1: 2 damage; pull 1
        t2: 4 damage; pull 2
        t3: 5 damage; pull 3
      - effect: If the target is pulled adjacent to the ensnarer, the ensnarer can make
          a free strike against them.
        name: Effect
```