---
agility: 2
ancestry:
- Undead
- Soulless
ev: 3 for four minions
file_basename: Decrepit Skeleton
file_dpath: Monsters/Undead/Statblocks
free_strike: 2
intuition: 0
item_id: decrepit-skeleton
item_index: '82'
item_name: Decrepit Skeleton
level: 1
might: 0
presence: -2
reason: -2
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster:decrepit-skeleton
scdc:
- 1.1.1:2:82
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '3'
type: monster
---

```ds-statblock
name: Decrepit Skeleton
level: 1
roles:
  - Minion Artillery
ancestry:
  - Undead
  - Soulless
ev: 3 for four minions
stamina: "3"
immunities:
  - Corruption 1
  - poison 1
speed: 5
size: 1M
stability: 0
free_strike: 2
with_captain: Gain an edge on strikes
might: 0
agility: 2
reason: -2
intuition: 0
presence: -2
traits:
  - name: Bonetrops
    effects:
      - effect: When the decrepit skeleton is reduced to 0 Stamina, their space is
          difficult terrain. The first time any enemy enters this space, the
          take 1 damage and the effect end.
abilities:
  - name: Bone Bow
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
      - effect: The decrepit skeleton chooses one other target within distance, who
          takes 1 damage.
        name: Effect
```