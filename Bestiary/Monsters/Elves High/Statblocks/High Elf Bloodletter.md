---
agility: 2
ancestry:
- Fey
- High Elf
- Humanoid
ev: '6'
file_basename: High Elf Bloodletter
file_dpath: Monsters/Elves High/Statblocks
free_strike: 4
intuition: 1
item_id: high-elf-bloodletter
item_index: '115'
item_name: High Elf Bloodletter
level: 1
might: 0
presence: 0
reason: 0
roles:
- Platoon Ambusher
scc:
- mcdm.monsters.v1:monster:high-elf-bloodletter
scdc:
- 1.1.1:2:115
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '30'
type: monster
---

```ds-statblock
name: High Elf Bloodletter
level: 1
roles:
  - Platoon Ambusher
ancestry:
  - Fey
  - High Elf
  - Humanoid
ev: "6"
stamina: "30"
speed: 7
size: 1M
stability: 0
free_strike: 4
might: 0
agility: 2
reason: 0
intuition: 1
presence: 0
traits:
  - name: Otherworldly Grace
    effects:
      - effect: At the start of each of their turns, the bloodletter can choose one
          effect on them that can be ended by a saving throw. That effect
          instead ends at the end of their turn.
abilities:
  - name: Razor's Edge
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 6 damage
        t2: 9 damage
        t3: 12 damage; R < 2 bleeding (save ends)
      - effect: The bloodletter and each of their allies has a double edge on abilities
          targeting a creature bleeding this way.
        name: Effect
  - name: Blood Haze
    cost: 2 Malice
    keywords:
      - Area
      - Magic
    type: Maneuver
    distance: 1 burst
    target: Special
    effects:
      - effect: Until the end of the next round, a cloud of blood vapor fills the area.
          The cloud blocks line of effect for enemies, and any enemy has damage
          weakness 3 while in the area. The bloodletter can then shift up to
          their speed, and can attempt to hide if they end that shift with
          concealment.
        name: Effect
```