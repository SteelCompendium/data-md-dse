---
agility: 1
ancestry:
- Eyestalk
- Horror
- Overmind
ev: '-'
file_basename: Mover Eye
file_dpath: Monsters/Xorannox the Tyract/Statblocks
free_strike: 3
intuition: 1
item_id: mover-eye
item_index: '317'
item_name: Mover Eye
level: 6
might: -1
presence: -1
reason: 4
roles:
- Controller
scc:
- mcdm.monsters.v1:monster:mover-eye
scdc:
- 1.1.1:2:317
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '30'
type: monster
---

```ds-statblock
name: Mover Eye
level: 6
roles:
  - Controller
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
      - effect: The mover eye has damage immunity 15. When they use a main action, they
          lose this immunity until the end of the round.
abilities:
  - name: Telekinetic Beam
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Psionic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 6
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        t1: 11 damage; slide 4
        t2: 17 damage; slide 5
        t3: 20 damage; slide 6
```