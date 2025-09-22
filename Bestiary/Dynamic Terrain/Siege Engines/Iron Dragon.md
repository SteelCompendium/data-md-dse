---
file_basename: Iron Dragon
file_dpath: Dynamic Terrain/Siege Engines
item_id: iron-dragon-level-4-siege-engine-artillery
item_index: '03'
item_name: Iron Dragon (Level 4 Siege Engine Artillery)
scc:
- mcdm.monsters.v1:dynamic-terrain.siege-engine:iron-dragon-level-4-siege-engine-artillery
scdc:
- 1.1.1:4.2:03
source: mcdm.monsters.v1
type: dynamic-terrain/siege-engine
---

~~~ds-featureblock
type: featureblock
featureblock_type: Siege Engine Artillery
name: Iron Dragon
level: 4
ev: "12"
flavor: A massive metal device uses a bellows system and liquid fuel to shoot
  out gouts of flame.
stamina: "60"
size: "2"
features:
  - type: feature
    feature_type: trait
    name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to an iron dragon can make an
          **Agility test**.
        tier1: The creature accidentally activates the **Gout of Flame** ability.
        tier2: The iron dragon is deactivated but the creature is slowed (EoT).
        tier3: The iron dragon is deactivated and can't be used.
  - type: feature
    feature_type: ability
    name: Gout of Flame
    icon: 🔳
    keywords:
      - Area
      - Weapon
    usage: Main action (Adjacent creature)
    distance: 8 x 2 line within 1
    target: Each creature and object in the area
    effects:
      - roll: Power Roll + 2
        tier1: 6 damage; A < 0 the target is burning (save ends)
        tier2: 10 damage; A < 1 the target is burning (save ends)
        tier3: 13 damage; A < 2 the target is burning (save ends)
      - name: Effect
        effect: A burning creature takes 1d6 fire damage at the start of each of their
          turns. A burning object takes 1d6 fire damage at the end of each
          round. This ability can't be used again until the iron dragon is
          reloaded.
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
        effect: The iron dragon is reloaded, allowing **Gout of Flame** to be used
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
        effect: The next use of **Gout of Flame** gains an edge and has a +10 bonus to
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
        effect: The iron dragon and the creature using this action move together up to 2
          squares.
~~~