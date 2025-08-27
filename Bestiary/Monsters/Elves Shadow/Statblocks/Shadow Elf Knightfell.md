---
agility: 2
ancestry:
- Fey
- Humanoid
- Shadow Elf
ev: '12'
file_basename: Shadow Elf Knightfell
file_dpath: Monsters/Elves Shadow/Statblocks
free_strike: 5
intuition: 3
item_id: shadow-elf-knightfell
item_index: '210'
item_name: Shadow Elf Knightfell
level: 4
might: 0
presence: 2
reason: 0
roles:
- Platoon Defender
scc:
- mcdm.monsters.v1:monster:shadow-elf-knightfell
scdc:
- 1.1.1:2:210
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '70'
type: monster
---

```ds-statblock
name: Shadow Elf Knightfell
level: 4
roles:
  - Platoon Defender
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
free_strike: 5
might: 0
agility: 2
reason: 0
intuition: 3
presence: 2
traits:
  - name: Of the Umbra
    effects:
      - effect: The knightfell ignores concealment created by darkness. While the
          knightfell is in direct sunlight, they have damage weakness 3. While
          the knightfell has concealment, they have damage immunity 3.
abilities:
  - name: Suffusing Strike
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 3
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        t1: 8 corruption damage
        t2: 12 corruption damage; R < 2 taunted (EoT)
        t3: 15 corruption damage; R < 3 taunted (EoT)
  - name: Trick of the Eye
    icon: ❗️
    keywords:
      - Magic
      - Melee
    type: Triggered action
    distance: Melee 2
    target: One ally
    trigger: An enemy within distance makes a strike against the target.
    effects:
      - effect: The target takes half the damage and the knightfell takes the other
          half.
        name: Effect
```