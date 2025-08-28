---
agility: 1
ancestry:
- Fey
- Humanoid
- Shadow Elf
ev: '12'
file_basename: Shadow Elf Luminator
file_dpath: Monsters/Elves Shadow/Statblocks
free_strike: 5
intuition: 3
item_id: shadow-elf-luminator
item_index: '213'
item_name: Shadow Elf Luminator
level: 4
might: 0
presence: 2
reason: 1
roles:
- Platoon Support
scc:
- mcdm.monsters.v1:monster:shadow-elf-luminator
scdc:
- 1.1.1:2:213
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '60'
type: monster
---

~~~ds-statblock
name: Shadow Elf Luminator
level: 4
roles:
  - Platoon Support
ancestry:
  - Fey
  - Humanoid
  - Shadow Elf
ev: "12"
stamina: "60"
speed: 5
movement: Climb
size: 1M
stability: 0
free_strike: 5
might: 0
agility: 1
reason: 1
intuition: 3
presence: 2
traits:
  - name: Of the Umbra
    effects:
      - effect: The luminator ignores concealment created by darkness. While the
          luminator is in direct sunlight, they have damage weakness 3. While
          the luminator has concealment, they have damage immunity 3.
abilities:
  - name: Lumina Mark
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
        t1: 8 lightning damage
        t2: 12 lightning damage
        t3: 15 lightning damage
      - effect: The next strike made against the target deals an extra 5 damage.
        name: Effect
  - name: Mourning Till Dusk
    icon: ❇️
    cost: 3 Malice
    keywords:
      - Area
      - Magic
    type: Main action
    distance: 2 burst
    target: Each ally in the area
    effects:
      - roll: Power Roll + 3
        t1: The target regains 6 Stamina.
        t2: The target regains 9 Stamina.
        t3: The target regains 12 Stamina and the Director gains 3 Malice.
      - effect: Each target gains an edge on their next strike.
        name: Effect
~~~