---
agility: 2
ancestry:
- Humanoid
- Kobold
ev: '3'
file_basename: Kobold Artifex
file_dpath: Monsters/Kobolds/Statblocks
free_strike: 1
intuition: 0
item_id: kobold-artifex
item_index: '91'
item_name: Kobold Artifex
level: 1
might: 0
presence: 0
reason: 1
roles:
- Horde Controller
scc:
- mcdm.monsters.v1:monster:kobold-artifex
scdc:
- 1.1.1:2:91
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '10'
type: monster
---

~~~ds-statblock
type: statblock
name: Kobold Artifex
level: 1
roles:
  - Horde Controller
ancestry:
  - Humanoid
  - Kobold
ev: "3"
stamina: "10"
speed: 5
size: 1S
stability: 0
free_strike: 1
might: 0
agility: 2
reason: 1
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Chain Hook
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 5
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 3 damage; pull 1
        tier2: 4 damage; pull 2
        tier3: 5 damage; pull 3
      - name: Effect
        effect: If this forced movement triggers a trap that uses a power roll, that
          roll has a double edge.
  - type: feature
    feature_type: ability
    name: Activate Trap
    icon: ⭐️
    keywords:
      - Ranged
    usage: Maneuver
    distance: Ranged 10
    target: One trap or other terrain object
    effects:
      - name: Effect
        effect: The trap or terrain object instantly triggers.
      - cost: 3 Malice
        effect: The artifex places a new trap in the encounter and can instantly trigger
          it. The artifex prefers working with angry beehives, flammable oil,
          snare traps, and spike traps (see Dynamic Terrain).
  - type: feature
    feature_type: trait
    name: Shield? Shield!
    icon: ⭐️
    effects:
      - effect: While adjacent to an ally who also has this trait, the artifex has
          stability 1, has cover, and grants cover to allies.
~~~