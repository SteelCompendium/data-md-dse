---
agility: 3
ancestry:
- Fey
- Humanoid
- Shadow Elf
ev: '14'
file_basename: Shadow Elf Moondancer
file_dpath: Monsters/Elves Shadow/Statblocks
free_strike: 6
intuition: 2
item_id: shadow-elf-moondancer
item_index: '211'
item_name: Shadow Elf Moondancer
level: 5
might: 1
presence: 0
reason: 1
roles:
- Platoon Harrier
scc:
- mcdm.monsters.v1:monster:shadow-elf-moondancer
scdc:
- 1.1.1:2:211
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '70'
type: monster
---

~~~ds-statblock
name: Shadow Elf Moondancer
level: 5
roles:
  - Platoon Harrier
ancestry:
  - Fey
  - Humanoid
  - Shadow Elf
ev: "14"
stamina: "70"
speed: 7
movement: Climb
size: 1M
stability: 0
free_strike: 6
might: 1
agility: 3
reason: 1
intuition: 2
presence: 0
traits:
  - name: Of the Umbra
    effects:
      - effect: The moondancer ignores concealment created by darkness. While the
          moondancer is in direct sunlight, they have damage weakness 3. While
          the moondancer has concealment, they have damage immunity 3.
abilities:
  - name: Crescent Sweep
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Charge
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
        t3: 16 damage
      - effect: Until the end of the current turn, the moondancer ignores opportunity
          attacks from the target.
        name: Effect
  - name: Dissolve
    icon: ❗️
    keywords:
      - Magic
    type: Triggered action
    distance: Self
    target: Self
    trigger: The moondancer takes damage from a strike.
    effects:
      - effect: The moondancer can teleport up to 10 squares to a space with concealment
          created by darkness.
        name: Effect
~~~