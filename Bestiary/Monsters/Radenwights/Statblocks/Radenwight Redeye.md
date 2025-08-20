---
agility: 2
ancestry:
- Humanoid
- Radenwight
ev: 3 for 4 minions
file_basename: Radenwight Redeye
file_dpath: Monsters/Radenwights/Statblocks
free_strike: 2
intuition: 0
item_id: radenwight-redeye
item_index: '155'
item_name: Radenwight Redeye
level: 1
might: 1
presence: 0
reason: -1
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster:radenwight-redeye
scdc:
- 1.1.1:2:155
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '3'
type: monster
---

```ds-statblock
name: Radenwight Redeye
level: 1
roles:
  - Minion Artillery
ancestry:
  - Humanoid
  - Radenwight
ev: 3 for 4 minions
stamina: "3"
speed: 5
movement: Climb
size: 1S
stability: 0
free_strike: 2
with_captain: Gain an edge on strikes
might: 1
agility: 2
reason: -1
intuition: 0
presence: 0
traits: []
abilities:
  - name: Eyes-On-Me-Shot
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
  - name: Ready Rodent
    keywords:
      - Melee
      - Weapon
    type: Triggered action
    distance: Melee 1
    target: One creature
    trigger: An ally deals damage to the target.
    effects:
      - effect: The redeye makes a free strike against the target.
```