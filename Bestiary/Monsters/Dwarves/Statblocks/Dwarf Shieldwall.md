---
agility: 0
ancestry:
- Dwarf
- Humanoid
ev: '10'
file_basename: Dwarf Shieldwall
file_dpath: Monsters/Dwarves/Statblocks
free_strike: 5
intuition: 0
item_id: dwarf-shieldwall
item_index: '405'
item_name: Dwarf Shieldwall
level: 3
might: 2
presence: 1
reason: 0
roles:
- Platoon Defender
scc:
- mcdm.monsters.v1:monster:dwarf-shieldwall
scdc:
- 1.1.1:2:405
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 4
stamina: '72'
type: monster
---

~~~ds-statblock
name: Dwarf Shieldwall
level: 3
roles:
  - Platoon Defender
ancestry:
  - Dwarf
  - Humanoid
ev: "10"
stamina: "72"
speed: 5
size: 1M
stability: 4
free_strike: 5
might: 2
agility: 0
reason: 0
intuition: 0
presence: 1
traits:
  - name: Call to the Wall
    effects:
      - effect: Whenever a creature deals damage to or takes damage from the shieldwall,
          the shieldwall can make that creature taunted until the end of the
          creature's next turn.
abilities:
  - name: Wide Axe
    icon: 🗡
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
        t1: 7 damage; slide 1
        t2: 10 damage; slide 1
        t3: 13 damage; slide 1
      - effect: The shieldwall can shift 1 square to remain adjacent to the target. A
          target restrained by a dwarf can be force moved by this ability. This
          forced movement doesn't end the restrained condition unless the
          Director determines otherwise.
        name: Effect
      - effect: This ability targets one additional target.
        cost: 3 Malice
  - name: Intercepting Shield
    icon: ❗️
    cost: 1 Malice
    keywords:
      - "-"
    type: Triggered action
    distance: Self
    target: Self
    trigger: A creature makes a strike against an ally adjacent to the shieldwall.
    effects:
      - effect: The shieldwall becomes the target of the triggering strike and halves
          the damage.
        name: Effect
~~~