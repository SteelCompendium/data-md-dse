---
agility: 2
ancestry:
- Fey
- Humanoid
- Shadow Elf
ev: '12'
file_basename: Shadow Elf Panther
file_dpath: Monsters/Elves Shadow/Statblocks
free_strike: 6
intuition: 1
item_id: shadow-elf-panther
item_index: '217'
item_name: Shadow Elf Panther
level: 4
might: 3
presence: 1
reason: -1
roles:
- Platoon Brute
scc:
- mcdm.monsters.v1:monster:shadow-elf-panther
scdc:
- 1.1.1:2:217
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '70'
type: monster
---

```ds-statblock
name: Shadow Elf Panther
level: 4
roles:
  - Platoon Brute
ancestry:
  - Fey
  - Humanoid
  - Shadow Elf
ev: "12"
stamina: "70"
speed: 5
movement: Climb
size: 1M
stability: 0
free_strike: 6
might: 3
agility: 2
reason: -1
intuition: 1
presence: 1
traits:
  - name: Of the Umbra
    effects:
      - effect: The panther ignores concealment created by darkness. While the panther
          is in direct sunlight, they have damage weakness 3. While the panther
          has concealment, they have damage immunity 3.
abilities:
  - name: Dusk Cleave
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        t1: 9 damage
        t2: 13 damage
        t3: 16 damage; I < 3 bleeding (save ends)
      - effect: The panther can make a free strike against a creature or object adjacent
          to the target.
        name: Effect
  - name: Bladestorm
    cost: 3 Malice
    keywords:
      - Area
      - Weapon
    type: Main action
    distance: 2 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        t1: 5 corruption damage
        t2: 8 corruption damage; I < 2 dazed (save ends)
        t3: 10 corruption damage; I < 3 dazed (save ends)
      - effect: The panther has a double edge on strikes against targets dazed this way.
        name: Effect
```