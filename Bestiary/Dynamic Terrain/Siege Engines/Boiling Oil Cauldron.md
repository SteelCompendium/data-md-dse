---
file_basename: Boiling Oil Cauldron
file_dpath: Dynamic Terrain/Siege Engines
item_id: boiling-oil-cauldron-level-3-fortification-defender
item_index: '01'
item_name: Boiling Oil Cauldron (Level 3 Fortification Defender)
scc:
- mcdm.monsters.v1:dynamic-terrain.siege-engine:boiling-oil-cauldron-level-3-fortification-defender
scdc:
- 1.1.1:4.2:01
source: mcdm.monsters.v1
type: dynamic-terrain/siege-engine
---

~~~ds-featureblock
type: featureblock
featureblock_type: Fortification Defender
name: Boiling Oil Cauldron
level: 3
ev: "10"
flavor: A large cauldron of boiling oil stands ready to be poured onto enemies.
stamina: "50"
size: 1L
features:
  - type: feature
    feature_type: trait
    name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to a boiling oil cauldron can make an
          **Agility test**.
        tier1: The creature accidentally activates the **Boiling Oil** ability.
        tier2: The boiling oil cauldron is deactivated but the creature is slowed (EoT).
        tier3: The boiling oil cauldron is deactivated and can't be used.
  - type: feature
    feature_type: ability
    name: Boiling Oil
    icon: 🔳
    keywords:
      - Area
      - Weapon
    usage: Main action (Adjacent creature)
    distance: 3 cube within 1
    target: Each creature and object in the area
    effects:
      - roll: Power Roll + 2
        tier1: 5 fire damage; M < 1 burning (save ends)
        tier2: 9 fire damage; M < 2 burning (save ends)
        tier3: 12 fire damage; M < 3 burning (save ends)
      - name: Effect
        effect: If the boiling oil is poured down on targets from above, it has high
          ground and gains an edge on the power roll. A burning creature takes
          1d6 fire damage at the start of each of their turns. A burning object
          takes 1d6 fire damage at the end of each round. This ability can't be
          used again until the boiling oil cauldron is reloaded.
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
        effect: The boiling oil cauldron is reloaded, allowing **Boiling Oil** to be
          used again. This action can be used only once per round.
~~~