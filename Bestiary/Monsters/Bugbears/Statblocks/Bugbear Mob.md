---
agility: -1
ancestry:
- Bugbear
- Fey
- Goblin
- Humanoid
ev: 7 for four minions
file_basename: Bugbear Mob
file_dpath: Monsters/Bugbears/Statblocks
free_strike: 3
intuition: 1
item_id: bugbear-mob
item_index: '289'
item_name: Bugbear Mob
level: 5
might: 3
presence: 0
reason: 0
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster:bugbear-mob
scdc:
- 1.1.1:2:289
size: '3'
source: mcdm.monsters.v1
speed: 6
stability: 2
stamina: '10'
type: monster
---

```ds-statblock
name: Bugbear Mob
level: 5
roles:
  - Minion Brute
ancestry:
  - Bugbear
  - Fey
  - Goblin
  - Humanoid
ev: 7 for four minions
stamina: "10"
speed: 6
size: "3"
stability: 2
free_strike: 3
with_captain: +2 damage bonus to strikes
might: 3
agility: -1
reason: 0
intuition: 1
presence: 0
traits:
  - name: Swarm
    effects:
      - effect: The mob can move through spaces as if they were a size 1L creature, and
          can occupy other creatures' spaces. At the start of each of the mob's
          turns, they can make a free strike against each creature whose space
          they share.
abilities:
  - name: Mug and Tear
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 3
        t1: 3 damage; pull 2
        t2: 6 damage; pull 3
        t3: 7 damage; pull 4, grabbed
      - effect: If the target is pulled into the mob, that forced movement deals damage
          only at the Director's determination.
        name: Effect
```