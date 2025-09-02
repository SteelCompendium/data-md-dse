---
file_basename: Lava
file_dpath: Dynamic Terrain/Environmental Hazards
item_id: lava-level-3-hazard-hexer
item_index: '07'
item_name: Lava (Level 3 Hazard Hexer)
scc:
- mcdm.monsters.v1:dynamic-terrain.environmental-hazard:lava-level-3-hazard-hexer
scdc:
- 1.1.1:4.5:07
source: mcdm.monsters.v1
type: dynamic-terrain/environmental-hazard
---

~~~ds-featureblock
name: Lava
type: Hazard Hexer
level: 3
ev: 4 per 10 x 10 patch
flavor: A patch of blisteringly hot molten rock wells up from the ground,
  threatening anyone who gets close to it.
stamina: 12 per square
size: One or more squares of difficult terrain
stats:
  - name: Immunity
    value: 20 to all damage except cold damage
features:
  - name: Deactivate
    icon: 🌀
    effects:
      - effect: Each square of lava must be individually destroyed.
  - name: Activate
    icon: ❕
    effects:
      - effect: A creature or object enters the lava or starts their turn there, or
          starts their turn adjacent to the lava.
      - effect: The **Liquid Hot Magma** ability.
        name: Effect
  - name: Liquid Hot Magma
    icon: ❗️
    keywords:
      - Melee
      - Strike
    type: Free triggered action
    distance: Melee 1
    target: The triggering creature or object
    trigger: A creature or object enters the lava or starts their turn there, or
      starts their turn adjacent to the lava.
    effects:
      - roll: Power Roll + 2
        t1: 5 fire damage; M < 1 the target is burning (save ends)
        t2: 9 fire damage; M < 2 the target is burning (save ends)
        t3: 12 fire damage; M < 3 the target is burning (save ends)
      - effect: If the target is adjacent to lava but not in it, this ability takes a
          bane. A burning creature takes 1d6 fire damage at the start of each of
          their turns. A burning object takes 1d6 fire damage at the end of each
          round.
        name: Effect
  - name: Upgrade
    icon: ⭐️
    effects:
      - effect: The lava is flowing! At the start of each round, add one square of lava
          adjacent to an existing square of lava.
        name: Magma Flow
        cost: +4 EV
~~~