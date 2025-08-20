---
agility: 1
ancestry:
- Eyestalk
- Horror
- Overmind
ev: '-'
file_basename: Necrotic Eye
file_dpath: Monsters/Xorannox the Tyract/Statblocks
free_strike: 3
intuition: 1
item_id: necrotic-eye
item_index: '321'
item_name: Necrotic Eye
level: 6
might: -1
presence: -1
reason: 4
roles:
- Hexer
scc:
- mcdm.monsters.v1:monster:necrotic-eye
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
name: Necrotic Eye
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
      - effect: The necrotic eye has damage immunity 15. When they use a main action,
          they lose this immunity until the end of the round.
abilities:
  - name: Necro Beam
    cost: Signature Ability
    keywords:
      - Psionic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        t1: 11 corruption damage
        t2: 17 corruption damage; M < 3 bleeding (save ends)
        t3: 20 corruption damage; M < 4 bleeding (save ends)
      - effect: If this damage or the Stamina loss from bleeding this way reduces a
          target creature's Stamina to 0, that creature dies.
```