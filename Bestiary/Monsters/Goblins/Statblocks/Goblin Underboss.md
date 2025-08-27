---
agility: 2
ancestry:
- Goblin
- Humanoid
ev: '3'
file_basename: Goblin Underboss
file_dpath: Monsters/Goblins/Statblocks
free_strike: 1
intuition: 0
item_id: goblin-underboss
item_index: '313'
item_name: Goblin Underboss
level: 1
might: -1
presence: 1
reason: 0
roles:
- Horde Support
scc:
- mcdm.monsters.v1:monster:goblin-underboss
scdc:
- 1.1.1:2:313
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '15'
type: monster
---

```ds-statblock
name: Goblin Underboss
level: 1
roles:
  - Horde Support
ancestry:
  - Goblin
  - Humanoid
ev: "3"
stamina: "15"
speed: 5
movement: Climb
size: 1S
stability: 0
free_strike: 1
might: -1
agility: 2
reason: 0
intuition: 0
presence: 1
traits:
  - name: Crafty
    effects:
      - effect: The underboss doesn't provoke opportunity attacks by moving.
abilities:
  - name: Swordplay
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 3 damage
        t2: 4 damage
        t3: 5 damage
      - effect: One ally adjacent to the target can make a free strike against them.
        name: Effect
  - name: Get Reckless!
    icon: ❇️
    keywords:
      - Area
    type: Maneuver
    distance: 5 burst
    target: Each ally in the area
    effects:
      - effect: Until the start of the underboss's next turn, each target gains an edge
          on strikes, and any strike made against a target gains an edge.
        name: Effect
      - effect: Strikes made against targets no longer gain an edge.
        cost: 2 Malice
```