---
agility: 2
ancestry:
- Dwarf
- Humanoid
ev: '6'
file_basename: Dwarf Gunner
file_dpath: Monsters/Dwarves/Statblocks
free_strike: 4
intuition: 1
item_id: dwarf-gunner
item_index: '404'
item_name: Dwarf Gunner
level: 1
might: 0
presence: 0
reason: 0
roles:
- Platoon Artillery
scc:
- mcdm.monsters.v1:monster:dwarf-gunner
scdc:
- 1.1.1:2:404
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '26'
type: monster
---

~~~ds-statblock
type: statblock
name: Dwarf Gunner
level: 1
roles:
  - Platoon Artillery
ancestry:
  - Dwarf
  - Humanoid
ev: "6"
stamina: "26"
speed: 5
size: 1M
stability: 1
free_strike: 4
might: 0
agility: 2
reason: 0
intuition: 1
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Portable Ballista
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 6 damage; push 1
        tier2: 9 damage; push 3
        tier3: 12 damage; push 5
      - name: Effect
        effect: If the target is adjacent to an object or a wall after the power roll is
          resolved, they are restrained until the end of their next turn. A
          target restrained by a dwarf can be force moved by this ability. This
          forced movement doesn't end the restrained condition unless the
          Director determines otherwise.
      - cost: 5 Malice
        effect: If the target is pushed into another creature, the target and the
          creature are each restrained until the end of their next turn.
  - type: feature
    feature_type: ability
    name: Ensnaring Chains
    icon: 🏹
    cost: 5 Malice
    keywords:
      - Ranged
      - Weapon
    usage: Maneuver
    distance: Ranged 10
    target: One prone, restrained, or slowed creature
    effects:
      - name: Effect
        effect: The gunner makes a free strike against the target, and the prone,
          restrained, and slowed conditions on the target end. The target is
          then restrained (save ends).
  - type: feature
    feature_type: trait
    name: Split Shot
    icon: ⭐️
    effects:
      - effect: Whenever the gunner deals rolled damage to a target, one creature or
          object adjacent to the target takes 3 damage.
~~~