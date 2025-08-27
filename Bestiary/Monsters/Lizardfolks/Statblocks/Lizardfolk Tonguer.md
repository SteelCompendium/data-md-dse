---
agility: 2
ancestry:
- Humanoid
- Lizardfolk
ev: 3 for four minions
file_basename: Lizardfolk Tonguer
file_dpath: Monsters/Lizardfolks/Statblocks
free_strike: 2
intuition: 1
item_id: lizardfolk-tonguer
item_index: '49'
item_name: Lizardfolk Tonguer
level: 1
might: 0
presence: 0
reason: 0
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster:lizardfolk-tonguer
scdc:
- 1.1.1:2:49
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '3'
type: monster
---

```ds-statblock
name: Lizardfolk Tonguer
level: 1
roles:
  - Minion Artillery
ancestry:
  - Humanoid
  - Lizardfolk
ev: 3 for four minions
stamina: "3"
speed: 5
movement: Swim
size: 1S
stability: 0
free_strike: 2
with_captain: +1 bonus to strikes
might: 0
agility: 2
reason: 0
intuition: 1
presence: 0
traits:
  - name: Reptilian Escape
    effects:
      - effect: While the tonguer has a tail, whenever they are grabbed, prone, slowed,
          or weakened, they can lose their tail to immediately end that
          condition, then shift up to 2 squares.
abilities:
  - name: Tonguelash
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 8
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        t1: 2 damage; pull 1, or the tonguer can shift 1 square toward the target
        t2: 4 damage; pull 2, or the tonguer shifts up to 2 squares toward the target
        t3: 5 damage; pull 3, or the tonguer shifts up to 3 squares toward the target
      - effect: If the forced movement or the shift leaves the target adjacent to the
          tonguer, the target is also grabbed.
        name: Effect
```