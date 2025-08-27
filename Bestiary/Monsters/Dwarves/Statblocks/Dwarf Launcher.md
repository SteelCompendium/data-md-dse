---
agility: 0
ancestry:
- Dwarf
- Humanoid
ev: '8'
file_basename: Dwarf Launcher
file_dpath: Monsters/Dwarves/Statblocks
free_strike: 4
intuition: 2
item_id: dwarf-launcher
item_index: '396'
item_name: Dwarf Launcher
level: 1
might: 1
presence: 0
reason: 0
roles:
- Platoon Hexer
scc:
- mcdm.monsters.v1:monster:dwarf-launcher
scdc:
- 1.1.1:2:396
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 3
stamina: '39'
type: monster
---

```ds-statblock
name: Dwarf Launcher
level: 1
roles:
  - Platoon Hexer
ancestry:
  - Dwarf
  - Humanoid
ev: "8"
stamina: "39"
speed: 5
size: 1M
stability: 3
free_strike: 4
might: 1
agility: 0
reason: 0
intuition: 2
presence: 0
traits:
  - name: Indirect Fire
    effects:
      - effect: The launcher ignores concealment and cover, and doesn't need line of
          effect to use their abilities as long as a size 1 opening exists
          between the dwarf and the target.
abilities:
  - name: Concussive Grenade
    icon: 🔳
    cost: Signature Ability
    keywords:
      - Area
      - Ranged
      - Weapon
    type: Main action
    distance: 3 cube within 5
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        t1: 3 damage; push 1
        t2: 6 damage; push 3; M < 1 slowed (save ends)
        t3: 8 damage; push 3; M < 2 slowed (save ends)
      - effect: A target restrained by a dwarf can be force moved by this ability. This
          forced movement doesn't end the restrained condition unless the
          Director determines otherwise.
        name: Effect
  - name: Sleep Grenade
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Ranged
      - Weapon
    type: Main action
    distance: 3 cube within 5
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        t1: 3 poison damage; I < 0 dazed (save ends)
        t2: 6 poison damage; I < 1 dazed (save ends)
        t3: 8 poison damage; I < 2 dazed (save ends)
      - effect: A target dazed this way treats their characteristic scores as 1 lower
          for the purpose of resisting potencies.
        name: Effect
```