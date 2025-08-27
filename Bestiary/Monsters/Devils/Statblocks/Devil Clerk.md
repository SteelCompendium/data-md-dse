---
agility: 0
ancestry:
- Devil
- Infernal
ev: 7 for four minions
file_basename: Devil Clerk
file_dpath: Monsters/Devils/Statblocks
free_strike: 3
intuition: 1
item_id: devil-clerk
item_index: '299'
item_name: Devil Clerk
level: 5
might: 3
presence: 2
reason: 1
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster:devil-clerk
scdc:
- 1.1.1:2:299
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '10'
type: monster
---

```ds-statblock
name: Devil Clerk
level: 5
roles:
  - Minion Brute
ancestry:
  - Devil
  - Infernal
ev: 7 for four minions
stamina: "10"
immunities:
  - Fire 5
speed: 6
size: 1M
stability: 0
free_strike: 3
with_captain: +2 damage bonus to strikes
might: 3
agility: 0
reason: 1
intuition: 1
presence: 2
traits:
  - name: True Name
    effects:
      - effect: If a creature within 10 squares speaks the clerk's true name, the clerk
          loses their fire immunity and any nondamaging effects of their
          signature ability until the end of the encounter.
abilities:
  - name: Quill Pushing
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
        t1: 3 damage; push 1
        t2: 6 damage; push 2
        t3: 7 damage; push 3
      - effect: Any target adjacent to two or more clerks is taunted until the end of
          their next turn.
        name: Effect
```