---
file_basename: Field Ballista
file_dpath: Dynamic Terrain/Siege Engines
item_id: field-ballista-level-2-siege-engine-artillery
item_index: '06'
item_name: Field Ballista (Level 2 Siege Engine Artillery)
scc:
- mcdm.monsters.v1:dynamic-terrain.siege-engine:field-ballista-level-2-siege-engine-artillery
scdc:
- 1.1.1:4.2:06
source: mcdm.monsters.v1
type: dynamic-terrain/siege-engine
---

~~~ds-featureblock
name: Field Ballista
type: Siege Engine Artillery
level: 2
ev: "8"
flavor: A massive crossbow fires thick metal bolts with devastating effect.
stamina: "40"
size: "2"
features:
  - name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to a field ballista can make an
          **Agility test**.
        t1: The creature accidentally activates the **Release Bolt** ability.
        t2: The field ballista is deactivated but the creature is slowed (EoT).
        t3: The field ballista is deactivated and can't be used.
  - name: Release Bolt
    icon: 🏹
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action (Adjacent creature)
    distance: Ranged 20
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 5 damage
        t2: 8 damage; M < 1 push 1
        t3: 11 damage; M < 2 push 2
      - effect: This ability can't be used again until the field ballista is reloaded.
        name: Effect
  - name: Reload
    icon: ⭐️
    keywords:
      - "-"
    type: Main action (Adjacent creature)
    distance: "-"
    target: "-"
    effects:
      - effect: The field ballista is reloaded, allowing **Release Bolt** to be used
          again. This action can be used only once per round.
        name: Effect
  - name: Spot
    icon: ⭐️
    keywords:
      - "-"
    type: Main action (Adjacent creature)
    distance: "-"
    target: "-"
    effects: []
  - name: Move
    icon: ⭐️
    keywords:
      - "-"
    type: Main action (Adjacent creature)
    distance: "-"
    target: "-"
    effects:
      - effect: The field ballista and the creature using this action move together up
          to 3 squares.
        name: Effect
  - name: Upgrades
    icon: ⭐️
    effects:
      - effect: The field ballista targets the nearest two additional creatures or
          objects in a straight line beyond the initial target.
        name: Penetrating Bolt
        cost: +2 EV
      - name: Chain Bolt
        cost: +2 EV
        effect: >-
          The field ballista's bolts are set with heavy chains that wrap around
          targets. The **Chain Bolt** ability replaces **Release Bolt**, and the
          field ballista gains the **Crank the Chain** ability.

          🏹 **Chain Bolt**

          | **- - Ranged, Strike, Weapon** | **Main action (Adjacent creature)**
          |

          | ------------------------------ | ----------------------------------:
          |

          | **📏 Ranged 20**               |       **🎯 One creature or object**
          |
      - roll: Power Roll + 2
        t1: 4 damage
        t2: 7 damage; M < 1 slowed (save ends)
        t3: 10 damage; M < 2 slowed (save ends)
      - name: Effect
        effect: |-
          This ability can't be used again until the field ballista is reloaded.
          🏹 **Crank the Chain**
          | **Ranged, Strike, Weapon** | **Main action (Adjacent creature)** |
          | -------------------------- | ----------------------------------: |
          | **📏 Ranged 20**           |                 **🎯 One creature** |
      - name: Special
        effect: The target must be slowed by the field ballista.
      - roll: Power Roll + 2
        t1: Pull 1
        t2: Pull
        t3: 3 Pull 5
      - effect: This forced movement triggers opportunity attacks.
        name: Effect
~~~