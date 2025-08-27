---
agility: 2
ancestry:
- Elemental
- High Elf
ev: 3 for four minions
file_basename: Soot Crow
file_dpath: Monsters/Elves High/Statblocks
free_strike: 1
intuition: 0
item_id: soot-crow
item_index: '117'
item_name: Soot Crow
level: 1
might: 0
presence: 1
reason: 0
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster:soot-crow
scdc:
- 1.1.1:2:117
size: 1T
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '4'
type: monster
---

```ds-statblock
name: Soot Crow
level: 1
roles:
  - Minion Harrier
ancestry:
  - Elemental
  - High Elf
ev: 3 for four minions
stamina: "4"
speed: 7
movement: Fly
size: 1T
stability: 0
free_strike: 1
with_captain: Gain an edge on strikes
might: 0
agility: 2
reason: 0
intuition: 0
presence: 1
traits: []
abilities:
  - name: Heckle
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
        t2: 2 damage
        t3: 3 damage; taunted (EoT)
      - effect: Until the end of their turn, the soot crow ignores opportunity attacks
          from the target.
        name: Effect
```