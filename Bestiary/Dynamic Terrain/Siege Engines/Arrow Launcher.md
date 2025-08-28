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
name: Arrow Launcher
type: Siege Engine Artillery
level: 2
ev: "8"
flavor: A small wooden cart uses alchemical rockets to launch up to a hundred
  arrows at a time across a wide area.
stamina: "30"
size: 1L
stats: []
features:
  - name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to an arrow launcher can make an
          **Agility test**.
        t1: The creature accidentally activates the **Arrow Storm** ability.
        t2: The arrow launcher is deactivated but the creature is slowed (EoT).
        t3: The arrow launcher is deactivated and can't be used.
  - name: Arrow Storm
    icon: 🔳
    keywords:
      - "- Area"
      - Ranged
      - Weapon
    type: Main action (Adjacent creature)
    distance: 5 cube within 20
    target: Each creature and object in the area
    effects:
      - roll: Power Roll + 2
        t1: 5 damage
        t2: 8 damage
        t3: 11 damage
      - effect: This ability can't be used again until the arrow launcher is reloaded.
        name: Effect
  - name: Reload
    icon: ⭐️
    keywords:
      - "-"
    type: Main action (Adjacent creature)
    distance: "-"
    target: "-"
    effects:
      - effect: The arrow launcher is reloaded, allowing **Arrow Storm** to be used
          again. This action can be used only once per round.
        name: Effect
  - name: Spot
    icon: ⭐️
    keywords:
      - "-"
    type: Main action (Adjacent creature)
    distance: "-"
    target: "-"
    effects:
      - effect: The next use of **Arrow Storm** gains an edge and has a +10 bonus to
          ranged distance. This action can be used only once per round.
        name: Effect
  - name: Move
    icon: ⭐️
    keywords:
      - "-"
    type: Main action (Adjacent creature)
    distance: "-"
    target: "-"
    effects:
      - effect: The arrow launcher and the creature using this action move together up
          to 3 squares.
        name: Effect
  - name: Upgrades
    icon: ⭐️
    effects:
      - effect: "**Flaming Arrows (+1 EV) Arrow Storm** deals fire damage, and can
          ignite flammable objects in its area."
      - effect: "**Screamers (+3 EV)** The arrows make a high-pitched screaming noise as
          they are fired and descend onto their targets. The **Screamers**
          ability replaces **Arrow Storm**."
  - name: Screamers
    icon: 🔳
    keywords:
      - Area
      - Ranged
      - Weapon
    type: Main action (Adjacent creature)
    distance: 5 cube within 20
    target: Each creature and object in the area
    effects:
      - cost: ≤11
        effect: 5 damage; R < 0 dazed (save ends)
        t2: 8 damage; R < 1 dazed (save ends)
        t3: 11 damage; R < 2 frightened (save ends)
      - effect: This ability can't be used again until the arrow
        name: Effect
      - effect: This ability can't be used again until the arrow launcher is reloaded.
        name: Effect
~~~