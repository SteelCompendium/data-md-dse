---
agility: 1
ancestry:
- Eyestalk
- Horror
- Overmind
ev: '-'
file_basename: Toxic Eye Level 6 Hexer
file_dpath: Monsters/Xorannox the Tyract/Statblocks
free_strike: 3
intuition: 1
item_id: toxic-eye-level-6-hexer
item_index: '322'
item_name: Toxic Eye Level 6 Hexer
level: 6
might: -1
presence: -1
reason: 4
roles:
- Hexer
scc:
- mcdm.monsters.v1:monster:toxic-eye-level-6-hexer
scdc:
- 1.1.1:2:322
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '30'
type: monster
---

```ds-statblock
name: Toxic Eye Level 6 Hexer
level: 6
roles:
  - Hexer
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
      - effect: The toxic eye has damage immunity 15. When they use a main action, they
          lose this immunity until the end of the round.
abilities:
  - name: Toxic Vapors
    cost: Signature Ability
    keywords:
      - Area
      - Psionic
      - Ranged
    type: Main action
    distance: 4 cube within 10
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        t1: 6 poison damage
        t2: 10 poison damage; M < 3 weakened (save ends)
        t3: 13 poison damage; M < 4 weakened (save ends)
```