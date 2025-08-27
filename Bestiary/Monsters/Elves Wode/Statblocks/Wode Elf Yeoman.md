---
agility: 2
ancestry:
- Fey
- Humanoid
- Wode Elf
ev: 3 for four minions
file_basename: Wode Elf Yeoman
file_dpath: Monsters/Elves Wode/Statblocks
free_strike: 2
intuition: 0
item_id: wode-elf-yeoman
item_index: '233'
item_name: Wode Elf Yeoman
level: 1
might: 0
presence: 1
reason: 0
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster:wode-elf-yeoman
scdc:
- 1.1.1:2:233
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '3'
type: monster
---

```ds-statblock
name: Wode Elf Yeoman
level: 1
roles:
  - Minion Artillery
ancestry:
  - Fey
  - Humanoid
  - Wode Elf
ev: 3 for four minions
stamina: "3"
speed: 7
size: 1M
stability: 0
free_strike: 2
with_captain: +1 damage bonus to strikes
might: 0
agility: 2
reason: 0
intuition: 0
presence: 1
traits:
  - name: Masking Glamor
    effects:
      - effect: Abilities targeting the yeoman that would take a bane from cover or
          concealment have a double bane instead.
abilities:
  - name: Heavy Longbow
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 12
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        t1: 2 damage; push 1
        t2: 4 damage; push 2
        t3: 5 damage; push 3
```