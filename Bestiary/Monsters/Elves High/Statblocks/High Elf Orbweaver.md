---
agility: 0
ancestry:
- Fey
- High Elf
- Humanoid
ev: '10'
file_basename: High Elf Orbweaver
file_dpath: Monsters/Elves High/Statblocks
free_strike: 5
intuition: 2
item_id: high-elf-orbweaver
item_index: '109'
item_name: High Elf Orbweaver
level: 3
might: 0
presence: 2
reason: 2
roles:
- Platoon Hexer
scc:
- mcdm.monsters.v1:monster:high-elf-orbweaver
scdc:
- 1.1.1:2:109
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '40'
type: monster
---

```ds-statblock
name: High Elf Orbweaver
level: 3
roles:
  - Platoon Hexer
ancestry:
  - Fey
  - High Elf
  - Humanoid
ev: "10"
stamina: "40"
speed: 5
size: 1M
stability: 0
free_strike: 5
might: 0
agility: 0
reason: 2
intuition: 2
presence: 2
traits:
  - name: Otherworldly Grace
    effects:
      - effect: At the start of each of their turns, the orbweaver can choose one effect
          on them that can be ended by a saving throw. That effect instead ends
          at the end of their turn.
abilities:
  - name: Awash
    cost: Signature Ability
    keywords:
      - Area
      - Magic
    type: Main action
    distance: 3 cube within 1
    target: Each creature in the area
    effects:
      - roll: Power Roll + 2
        t1: 4 cold damage; M < 0 push 3
        t2: 6 cold damage; M < 1 push 5 or prone
        t3: 9 cold damage; M < 2 slide 5 or prone
  - name: Aetherweb
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 8
    target: Two enemies or objects
    effects:
      - roll: Power Roll + 2
        t1: 5 damage; R < 0 slowed (save ends)
        t2: 8 damage; R < 1 slowed (save ends)
        t3: 11 damage; R < 2 restrained (save ends)
      - effect: Each enemy within 3 squares of a target suffers the same potency effect
          as the target unless they are already adjacent to them, or if they
          immediately shift into an unoccupied space adjacent to the target (no
          action required).
        name: Effect
```