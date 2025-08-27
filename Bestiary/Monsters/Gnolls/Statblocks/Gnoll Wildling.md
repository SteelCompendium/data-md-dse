---
agility: 2
ancestry:
- Abyssal
- Gnoll
ev: 4 for four minions
file_basename: Gnoll Wildling
file_dpath: Monsters/Gnolls/Statblocks
free_strike: 2
intuition: 0
item_id: gnoll-wildling
item_index: '42'
item_name: Gnoll Wildling
level: 2
might: 1
presence: -2
reason: 0
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster:gnoll-wildling
scdc:
- 1.1.1:2:42
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 1
stamina: '5'
type: monster
---

```ds-statblock
name: Gnoll Wildling
level: 2
roles:
  - Minion Harrier
ancestry:
  - Abyssal
  - Gnoll
ev: 4 for four minions
stamina: "5"
speed: 7
size: 1M
stability: 1
free_strike: 2
with_captain: Gain an edge on strikes
might: 1
agility: 2
reason: 0
intuition: 0
presence: -2
traits:
  - name: Death Circle
    effects:
      - effect: Whenever a non-minion ally within 7 squares of the wildling is reduced
          to 0 Stamina, the wildling can move up to their speed.
abilities:
  - name: Flail
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
        t1: 2 damage
        t2: 3 damage
        t3: 5 damage; the wildling can make a free strike against a creature adjacent to
          the target
```