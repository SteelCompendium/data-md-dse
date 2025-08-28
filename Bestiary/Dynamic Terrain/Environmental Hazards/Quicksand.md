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
name: Quicksand
type: Hazard Hexer
level: 3
ev: 3 per 10 x 10 patch
flavor: When this patch of sand is stepped on, it is revealed to be a slurry
  saturated by water-and ready to draw creatures down to their doom.
stamina: "-"
size: One or more squares
stats: []
features:
  - name: Deactivate
    icon: 🌀
    effects: []
  - name: Activate
    icon: ❕
    effects:
      - effect: A creature or object enters the quicksand or starts their turn there.
      - effect: The **Grasping Depths** ability.
        name: Effect
  - name: Grasping Depths
    icon: ❗️
    keywords:
      - Melee
      - Strike
    type: Free triggered action
    distance: Melee 0
    target: The triggering creature or object
    trigger: A creature or object enters the quicksand or starts their turn there.
    effects:
      - roll: Power Roll + 2
        t1: M < 0 slowed (save ends)
        t2: M < 1 restrained (save ends)
        t3: M < 2 restrained (save ends)
      - effect: This ability takes a bane if a triggering creature shifted into the
          quicksand. A character who starts their turn restrained this way is
          suffocating.
        name: Effect
  - name: Hidden
    icon: ⭐️
    effects:
      - effect: The quicksand is hidden until triggered or detected.
~~~