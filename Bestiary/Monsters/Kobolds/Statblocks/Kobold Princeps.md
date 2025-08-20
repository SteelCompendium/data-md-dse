---
agility: 2
ancestry:
- Humanoid
- Kobold
ev: 3 for four minions
file_basename: Kobold Princeps
file_dpath: Monsters/Kobolds/Statblocks
free_strike: 1
intuition: 0
item_id: kobold-princeps
item_index: '92'
item_name: Kobold Princeps
level: 1
might: 0
presence: 0
reason: 0
roles:
- Minion Support
scc:
- mcdm.monsters.v1:monster:kobold-princeps
scdc:
- 1.1.1:2:92
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '4'
type: monster
---

```ds-statblock
name: Kobold Princeps
level: 1
roles:
  - Minion Support
ancestry:
  - Humanoid
  - Kobold
ev: 3 for four minions
stamina: "4"
speed: 5
size: 1S
stability: 0
free_strike: 1
with_captain: +2 bonus to Stamina
might: 0
agility: 2
reason: 0
intuition: 0
presence: 0
traits:
  - name: Shield? Shield!
    effects:
      - effect: While adjacent to an ally who also has this trait, the princeps has
          stability 1, has cover, and grants cover to allies.
abilities:
  - name: Hasta
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        t1: 1 damage
        t2: 2 damage
        t3: 3 damage
      - effect: One ally within 3 squares of the princeps shifts up to 2 squares
```