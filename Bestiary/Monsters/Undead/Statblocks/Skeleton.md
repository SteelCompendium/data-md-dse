---
agility: 2
ancestry:
- Undead
- Soulless
ev: '3'
file_basename: Skeleton
file_dpath: Monsters/Undead/Statblocks
free_strike: 2
intuition: 0
item_id: skeleton
item_index: '84'
item_name: Skeleton
level: 1
might: 0
presence: -1
reason: 1
roles:
- Horde Artillery
scc:
- mcdm.monsters.v1:monster:skeleton
scdc:
- 1.1.1:2:84
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '10'
type: monster
---

```ds-statblock
name: Skeleton
level: 1
roles:
  - Horde Artillery
ancestry:
  - Undead
  - Soulless
ev: "3"
stamina: "10"
immunities:
  - Corruption 1
  - poison 1
speed: 5
size: 1M
stability: 0
free_strike: 2
might: 0
agility: 2
reason: 1
intuition: 0
presence: -1
traits:
  - name: Arise
    effects:
      - effect: The first time the skeleton is reduced to 0 Stamina by damage that isn't
          fire damage or holy damage and their body isn't destroyed, they
          instead have 1 Stamina and fall prone.
abilities:
  - name: Bone Shards
    cost: Signature Ability
    keywords:
      - Melee
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1 or ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 4 damage
        t2: 6 damage
        t3: 7 damage
      - effect: Until the start of the skeleton's next turn, the target takes 2 damage
          the first time they willingly move on their turn
        name: Effect
  - name: Bone Spur
    cost: 2 Malice
    keywords:
      - Area
      - Weapon
    type: Maneuver
    distance: 1 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        t1: 1 damage; M < 0 bleeding (save ends)
        t2: 2 damage; M < 1 bleeding (save ends)
        t3: 3 damage; M < 2 bleeding (save ends)
      - effect: Each target takes a bane on their next strike.
        name: Effect
```