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
type: featureblock
featureblock_type: Siege Engine Artillery
name: Field Ballista
level: 2
ev: "8"
flavor: A massive crossbow fires thick metal bolts with devastating effect.
stamina: "40"
size: "2"
features:
  - type: feature
    feature_type: trait
    name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to a field ballista can make an
          **Agility test**.
        tier1: The creature accidentally activates the **Release Bolt** ability.
        tier2: The field ballista is deactivated but the creature is slowed (EoT).
        tier3: The field ballista is deactivated and can't be used.
  - type: feature
    feature_type: ability
    name: Release Bolt
    icon: 🏹
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action (Adjacent creature)
    distance: Ranged 20
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 5 damage
        tier2: 8 damage; M < 1 push 1
        tier3: 11 damage; M < 2 push 2
      - name: Effect
        effect: This ability can't be used again until the field ballista is reloaded.
  - type: feature
    feature_type: ability
    name: Reload
    icon: ⭐️
    keywords:
      - "-"
    usage: Main action (Adjacent creature)
    distance: "-"
    target: "-"
    effects:
      - name: Effect
        effect: The field ballista is reloaded, allowing **Release Bolt** to be used
          again. This action can be used only once per round.
  - type: feature
    feature_type: ability
    name: Spot
    icon: ⭐️
    keywords:
      - "-"
    usage: Main action (Adjacent creature)
    distance: "-"
    target: "-"
    effects: []
  - type: feature
    feature_type: ability
    name: Move
    icon: ⭐️
    keywords:
      - "-"
    usage: Main action (Adjacent creature)
    distance: "-"
    target: "-"
    effects:
      - name: Effect
        effect: The field ballista and the creature using this action move together up
          to 3 squares.
  - type: feature
    feature_type: trait
    name: Upgrades
    icon: ⭐️
    effects:
      - name: Penetrating Bolt
        cost: +2 EV
        effect: The field ballista targets the nearest two additional creatures or
          objects in a straight line beyond the initial target.
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
        tier1: 4 damage
        tier2: 7 damage; M < 1 slowed (save ends)
        tier3: 10 damage; M < 2 slowed (save ends)
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
        tier1: Pull 1
        tier2: Pull
        tier3: 3 Pull 5
      - name: Effect
        effect: This forced movement triggers opportunity attacks.
~~~