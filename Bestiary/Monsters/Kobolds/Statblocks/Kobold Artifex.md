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
traits:
  - name: Shield? Shield!
    effects:
      - effect: While adjacent to an ally who also has this trait, the artifex has
          stability 1, has cover, and grants cover to allies.
abilities:
  - name: Chain Hook
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 5
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 3 damage; pull 1
        t2: 4 damage; pull 2
        t3: 5 damage; pull 3
      - effect: If this forced movement triggers a trap that uses a power roll, that
          roll has a double edge.
        name: Effect
  - name: Activate Trap
    icon: ⭐️
    keywords:
      - Ranged
    type: Maneuver
    distance: Ranged 10
    target: One trap or other terrain object
    effects:
      - effect: The trap or terrain object instantly triggers.
        name: Effect
      - effect: The artifex places a new trap in the encounter and can instantly trigger
          it. The artifex prefers working with angry beehives, flammable oil,
          snare traps, and spike traps (see Dynamic Terrain).
        cost: 3 Malice
~~~