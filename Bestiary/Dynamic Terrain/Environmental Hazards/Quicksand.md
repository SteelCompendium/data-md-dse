---
file_basename: Quicksand
file_dpath: Dynamic Terrain/Environmental Hazards
item_id: quicksand-level-3-hazard-hexer
item_index: '01'
item_name: Quicksand (Level 3 Hazard Hexer)
scc:
- mcdm.monsters.v1:dynamic-terrain.environmental-hazard:quicksand-level-3-hazard-hexer
scdc:
- 1.1.1:4.5:01
source: mcdm.monsters.v1
type: dynamic-terrain/environmental-hazard
---

~~~ds-featureblock
type: featureblock
featureblock_type: Hazard Hexer
name: Quicksand
level: 3
ev: 3 per 10 x 10 patch
flavor: When this patch of sand is stepped on, it is revealed to be a slurry
  saturated by water-and ready to draw creatures down to their doom.
stamina: "-"
size: One or more squares
features:
  - type: feature
    feature_type: trait
    name: Deactivate
    icon: 🌀
    effects: []
  - type: feature
    feature_type: trait
    name: Activate
    icon: ❕
    effects:
      - effect: A creature or object enters the quicksand or starts their turn there.
      - name: Effect
        effect: The **Grasping Depths** ability.
  - type: feature
    feature_type: ability
    name: Grasping Depths
    icon: ❗️
    keywords:
      - Melee
      - Strike
    usage: Free triggered action
    distance: Melee 0
    target: The triggering creature or object
    trigger: A creature or object enters the quicksand or starts their turn there.
    effects:
      - roll: Power Roll + 2
        tier1: M < 0 slowed (save ends)
        tier2: M < 1 restrained (save ends)
        tier3: M < 2 restrained (save ends)
      - name: Effect
        effect: This ability takes a bane if a triggering creature shifted into the
          quicksand. A character who starts their turn restrained this way is
          suffocating.
  - type: feature
    feature_type: trait
    name: Hidden
    icon: ⭐️
    effects:
      - effect: The quicksand is hidden until triggered or detected.
~~~