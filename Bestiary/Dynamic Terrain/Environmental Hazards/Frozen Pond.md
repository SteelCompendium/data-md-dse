---
file_basename: Frozen Pond
file_dpath: Dynamic Terrain/Environmental Hazards
item_id: frozen-pond-level-1-hazard-hexer
item_index: '06'
item_name: Frozen Pond (Level 1 Hazard Hexer)
scc:
- mcdm.monsters.v1:dynamic-terrain.environmental-hazard:frozen-pond-level-1-hazard-hexer
scdc:
- 1.1.1:4.5:06
source: mcdm.monsters.v1
type: dynamic-terrain/environmental-hazard
---

~~~ds-featureblock
type: featureblock
featureblock_type: Hazard Hexer
name: Frozen Pond
level: 1
ev: 1 per 10 x 10 pond
flavor: A shallow, frozen patch of water features ice thick enough that it won't
  break, but its surface is slick and treacherous to navigate.
stamina: 3 per square
size: One or more squares of difficult terrain
stats:
  - name: Immunity
    value: 5 to all damage except fire damage
features:
  - type: feature
    feature_type: trait
    name: Deactivate
    icon: 🌀
    effects:
      - effect: Destroying a square of the frozen pond turns the square into shallow icy
          water.
  - type: feature
    feature_type: trait
    name: Activate
    icon: ❕
    effects:
      - effect: A creature or object enters a square of the frozen pond without
          shifting.
      - name: Effect
        effect: The **Slippery Surface** ability.
  - type: feature
    feature_type: ability
    name: Slippery Surface
    icon: ❗️
    keywords:
      - Melee
      - Strike
    usage: Free triggered action
    distance: Melee 0
    target: The triggering creature or object
    trigger: A creature or object enters a square of the frozen pond without shifting.
    effects:
      - roll: Power Roll + 2
        tier1: Push 1 in the direction the target was moving
        tier2: Push 2 in the direction the target was moving; A < 1 slowed (save ends)
        tier3: Push 3 in the direction the target was moving; A < 2 prone and can't
          stand (save ends)
      - name: Effect
        effect: The triggering creature's movement ends, then they are force moved. If
          the target triggered this ability by being force moved, this ability
          gains an edge and any remaining forced movement distance is added to
          the ability's forced movement. The ability's forced movement doesn't
          trigger the ability again.
  - type: feature
    feature_type: trait
    name: Upgrade
    icon: ⭐️
    effects:
      - name: Thin Ice
        cost: +1 EV
        effect: >-
          The ice covering the pond is thin and the water is deeper. Whenever a
          creature or object enters or falls prone in a square of the frozen
          pond, that square is destroyed and replaced with icy water. The **Icy
          Water** ability replaces **Slippery Surface**.

          Any creature who starts their turn in the icy water takes 1 cold
          damage. If the water is deep enough, a creature can swim beneath the
          surface of the frozen pond, but takes this cold damage while doing so.
  - type: feature
    feature_type: ability
    name: "Power Roll + 2:"
    keywords:
      - Melee
      - Strike
    usage: Free triggered action
    distance: Melee 0
    target: The triggering creature or object
    trigger: A creature or object enters or falls prone in a square of the frozen pond.
    effects:
      - tier1: Slide 1
        tier2: 1 cold damage; M < 1 slowed (save ends)
        tier3: 3 cold damage; M < 2 restrained (save ends)
      - name: Effect
        effect: The triggering creature's movement ends, then they are force moved if
          applicable.
~~~