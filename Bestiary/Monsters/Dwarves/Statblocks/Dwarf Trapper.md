---
agility: 2
ancestry:
- Dwarf
- Humanoid
ev: '6'
file_basename: Dwarf Trapper
file_dpath: Monsters/Dwarves/Statblocks
free_strike: 3
intuition: 1
item_id: dwarf-trapper
item_index: '402'
item_name: Dwarf Trapper
level: 1
might: 0
presence: 0
reason: 0
roles:
- Platoon Harrier
scc:
- mcdm.monsters.v1:monster:dwarf-trapper
scdc:
- 1.1.1:2:402
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 2
stamina: '36'
type: monster
---

~~~ds-statblock
name: Dwarf Trapper
level: 1
roles:
  - Platoon Harrier
ancestry:
  - Dwarf
  - Humanoid
ev: "6"
stamina: "36"
speed: 7
size: 1M
stability: 2
free_strike: 3
might: 0
agility: 2
reason: 0
intuition: 1
presence: 0
traits: []
abilities:
  - name: Concussive Bolts
    icon: ⚔️
    cost: Signature Ability
    keywords:
      - Charge
      - Melee
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1 or ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 5 damage; push 2
        t2: 7 damage; push 4
        t3: 9 damage; push 6
      - effect: A target restrained by a dwarf can be force moved by this ability. This
          forced movement doesn't end the restrained condition unless the
          Director determines otherwise.
        name: Effect
  - name: Steam-Powered Snare
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
      - Ranged
      - Weapon
    type: Maneuver
    distance: 3 cube within 5
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: Each target makes a **Might test**.
        t1: 7 damage; restrained (EoT)
        t2: 5 damage; slowed (EoT)
        t3: No effect.
      - effect: The snare remains until the end of the encounter. Any enemy who moves
          into the area for the first time in a round or starts their turn there
          must make the test.
~~~