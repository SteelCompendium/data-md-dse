---
agility: 2
ancestry:
- Humanoid
- Lizardfolk
ev: 3 for four minions
file_basename: Lizardfolk Grunt
file_dpath: Monsters/Lizardfolks/Statblocks
free_strike: 1
intuition: 0
item_id: lizardfolk-grunt
item_index: '50'
item_name: Lizardfolk Grunt
level: 1
might: 1
presence: 0
reason: 0
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster:lizardfolk-grunt
scdc:
- 1.1.1:2:50
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '4'
type: monster
---

```ds-statblock
name: Lizardfolk Grunt
level: 1
roles:
  - Minion Harrier
ancestry:
  - Humanoid
  - Lizardfolk
ev: 3 for four minions
stamina: "4"
speed: 6
movement: Swim
size: 1M
stability: 0
free_strike: 1
with_captain: +2 bonus to speed
might: 1
agility: 2
reason: 0
intuition: 0
presence: 0
traits:
  - name: Reptilian Escape
    effects:
      - effect: While the grunt has a tail, whenever they are grabbed, prone, slowed, or
          weakened, they can lose their tail to immediately end that condition,
          then shift up to 2 squares.
abilities:
  - name: Snap and Toss
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
      - roll: Power Roll + 2
        t1: 1 damage
        t2: 2 damage; slide 2
        t3: 3 damage; slide 2
```