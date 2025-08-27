---
agility: 1
ancestry:
- Fey
- Humanoid
- Shadow Elf
ev: 6 for four minions
file_basename: Shadow Elf Cloak
file_dpath: Monsters/Elves Shadow/Statblocks
free_strike: 2
intuition: 0
item_id: shadow-elf-cloak
item_index: '212'
item_name: Shadow Elf Cloak
level: 4
might: 3
presence: 0
reason: 0
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster:shadow-elf-cloak
scdc:
- 1.1.1:2:212
size: 1M
source: mcdm.monsters.v1
speed: 8
stability: 0
stamina: '8'
type: monster
---

```ds-statblock
name: Shadow Elf Cloak
level: 4
roles:
  - Minion Harrier
ancestry:
  - Fey
  - Humanoid
  - Shadow Elf
ev: 6 for four minions
stamina: "8"
speed: 8
movement: Climb
size: 1M
stability: 0
free_strike: 2
with_captain: +2 bonus to speed
might: 3
agility: 1
reason: 0
intuition: 0
presence: 0
traits:
  - name: Of the Umbra
    effects:
      - effect: The cloak ignores concealment created by darkness. While the cloak is in
          direct sunlight, they have damage weakness 3. While the cloak has
          concealment, they have damage immunity 3.
abilities:
  - name: Stick and Poke
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
        t1: 2 damage
        t2: 4 damage
        t3: 6 damage
      - effect: The cloak shifts up to 2 squares
        name: Effect
```