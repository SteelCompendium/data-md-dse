---
agility: 1
ancestry:
- Eyestalk
- Horror
- Overmind
ev: '-'
file_basename: Demolition
file_dpath: Monsters/Xorannox the Tyract/Statblocks
free_strike: 3
intuition: 1
item_id: demolition
item_index: '321'
item_name: Demolition
level: 6
might: -1
presence: -1
reason: 4
roles:
- Artillery
scc:
- mcdm.monsters.v1:monster:demolition
scdc:
- 1.1.1:2:321
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '30'
type: monster
---

```ds-statblock
name: Demolition
level: 6
roles:
  - Artillery
ancestry:
  - Eyestalk
  - Horror
  - Overmind
ev: "-"
stamina: "30"
speed: 5
movement: Fly, hover
size: 1M
stability: 0
free_strike: 3
might: -1
agility: 1
reason: 4
intuition: 1
presence: -1
traits:
  - name: Psionic Barrier
    effects:
      - effect: The demolition eye has damage immunity 15. When they use a main action,
          they lose this immunity until the end of the round.
abilities:
  - name: Explosion
    icon: 🔳
    cost: Signature Ability
    keywords:
      - Psionic
      - Ranged
      - Strike
    type: Main action
    distance: 4 cube within 10
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        t1: 6 fire damage
        t2: 10 fire damage; M < 3 prone
        t3: 13 fire damage; M < 4 prone
```