---
file_basename: Arrow Launcher
file_dpath: Dynamic Terrain/Siege Engines
item_id: arrow-launcher-level-2-siege-engine-artillery
item_index: '02'
item_name: Arrow Launcher (Level 2 Siege Engine Artillery)
scc:
- mcdm.monsters.v1:dynamic-terrain.siege-engine:arrow-launcher-level-2-siege-engine-artillery
scdc:
- 1.1.1:4.2:02
source: mcdm.monsters.v1
type: dynamic-terrain/siege-engine
---

~~~ds-featureblock
type: featureblock
featureblock_type: Siege Engine Artillery
name: Arrow Launcher
level: 2
ev: "8"
flavor: A small wooden cart uses alchemical rockets to launch up to a hundred
  arrows at a time across a wide area.
stamina: "30"
size: 1L
features:
  - type: feature
    feature_type: trait
    name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to an arrow launcher can make an
          **Agility test**.
        tier1: The creature accidentally activates the **Arrow Storm** ability.
        tier2: The arrow launcher is deactivated but the creature is slowed (EoT).
        tier3: The arrow launcher is deactivated and can't be used.
  - type: feature
    feature_type: ability
    name: Arrow Storm
    icon: 🔳
    keywords:
      - "- Area"
      - Ranged
      - Weapon
    usage: Main action (Adjacent creature)
    distance: 5 cube within 20
    target: Each creature and object in the area
    effects:
      - roll: Power Roll + 2
        tier1: 5 damage
        tier2: 8 damage
        tier3: 11 damage
      - name: Effect
        effect: This ability can't be used again until the arrow launcher is reloaded.
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
        effect: The arrow launcher is reloaded, allowing **Arrow Storm** to be used
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
    effects:
      - name: Effect
        effect: The next use of **Arrow Storm** gains an edge and has a +10 bonus to
          ranged distance. This action can be used only once per round.
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
        effect: The arrow launcher and the creature using this action move together up
          to 3 squares.
  - type: feature
    feature_type: trait
    name: Upgrades
    icon: ⭐️
    effects:
      - name: Flaming Arrows
        cost: +1 EV
        effect: deals fire damage, and can ignite flammable objects in its area.
      - name: Screamers
        cost: +3 EV
        effect: The arrows make a high-pitched screaming noise as they are fired and
          descend onto their targets. The **Screamers** ability replaces **Arrow
          Storm**.
  - type: feature
    feature_type: ability
    name: Screamers
    icon: 🔳
    keywords:
      - Area
      - Ranged
      - Weapon
    usage: Main action (Adjacent creature)
    distance: 5 cube within 20
    target: Each creature and object in the area
    effects:
      - roll: Power Roll + 2
        tier1: 5 damage; R < 0 dazed (save ends)
        tier2: 8 damage; R < 1 dazed (save ends)
        tier3: 11 damage; R < 2 frightened (save ends)
      - name: Effect
        effect: This ability can't be used again until the arrow
      - name: Effect
        effect: This ability can't be used again until the arrow launcher is reloaded.
~~~