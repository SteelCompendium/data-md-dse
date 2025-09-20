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
item_index: '407'
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
- 1.1.1:2:407
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 4
stamina: '72'
type: monster
---

~~~ds-statblock
type: statblock
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
features:
  - type: feature
    feature_type: ability
    name: Wide Axe
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 7 damage; slide 1
        tier2: 10 damage; slide 1
        tier3: 13 damage; slide 1
      - name: Effect
        effect: The shieldwall can shift 1 square to remain adjacent to the target. A
          target restrained by a dwarf can be force moved by this ability. This
          forced movement doesn't end the restrained condition unless the
          Director determines otherwise.
      - cost: 3 Malice
        effect: This ability targets one additional target.
  - type: feature
    feature_type: ability
    name: Intercepting Shield
    icon: ❗️
    cost: 1 Malice
    keywords:
      - "-"
    usage: Triggered action
    distance: Self
    target: Self
    trigger: A creature makes a strike against an ally adjacent to the shieldwall.
    effects:
      - name: Effect
        effect: The shieldwall becomes the target of the triggering strike and halves
          the damage.
  - type: feature
    feature_type: trait
    name: Call to the Wall
    icon: ⭐️
    effects:
      - effect: Whenever a creature deals damage to or takes damage from the shieldwall,
          the shieldwall can make that creature taunted until the end of the
          creature's next turn.
~~~