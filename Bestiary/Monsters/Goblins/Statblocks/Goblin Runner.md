---
agility: 2
ancestry:
- Goblin
- Humanoid
ev: 3 for four minions
file_basename: Goblin Runner
file_dpath: Monsters/Goblins/Statblocks
free_strike: 1
intuition: 0
item_id: goblin-runner
item_index: '311'
item_name: Goblin Runner
level: 1
might: -2
presence: -1
reason: 0
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster:goblin-runner
scdc:
- 1.1.1:2:311
size: 1S
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '4'
type: monster
---

~~~ds-statblock
name: Goblin Runner
level: 1
roles:
  - Minion Harrier
ancestry:
  - Goblin
  - Humanoid
ev: 3 for four minions
stamina: "4"
speed: 6
movement: Climb
size: 1S
stability: 0
free_strike: 1
with_captain: Gain an edge on strikes
might: -2
agility: 2
reason: 0
intuition: 0
presence: -1
traits:
  - name: Crafty
    effects:
      - effect: The runner doesn't provoke opportunity attacks by moving
abilities:
  - name: Club Charge
    icon: 🗡
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
      - roll: Power Roll + 2
        t1: 1 damage
        t2: 2 damage
        t3: 3 damage
~~~