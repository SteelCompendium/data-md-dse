---
agility: 2
ancestry:
- Goblin
- Humanoid
ev: 3 for four minions
file_basename: Goblin Sniper
file_dpath: Monsters/Goblins/Statblocks
free_strike: 2
intuition: 0
item_id: goblin-sniper
item_index: '315'
item_name: Goblin Sniper
level: 1
might: -2
presence: -1
reason: 0
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster:goblin-sniper
scdc:
- 1.1.1:2:315
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '3'
type: monster
---

```ds-statblock
name: Goblin Sniper
level: 1
roles:
  - Minion Artillery
ancestry:
  - Goblin
  - Humanoid
ev: 3 for four minions
stamina: "3"
speed: 5
movement: Climb
size: 1S
stability: 0
free_strike: 2
with_captain: +5 bonus to ranged distance
might: -2
agility: 2
reason: 0
intuition: 0
presence: -1
traits:
  - name: Crafty
    effects:
      - effect: The sniper doesn't provoke opportunity attacks by moving.
abilities:
  - name: Bow
    cost: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 10
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        t1: 2 damage
        t2: 4 damage
        t3: 5 damage
      - effect: If the sniper doesn't use a move action this turn, this ability gains an
          edge.
```