---
file_basename: Corrosive Pool
file_dpath: Dynamic Terrain/Environmental Hazards
item_id: corrosive-pool-level-2-hazard-hexer
item_index: '02'
item_name: Corrosive Pool (Level 2 Hazard Hexer)
scc:
- mcdm.monsters.v1:dynamic-terrain.environmental-hazard:corrosive-pool-level-2-hazard-hexer
scdc:
- 1.1.1:4.5:02
source: mcdm.monsters.v1
type: dynamic-terrain/environmental-hazard
---

~~~ds-featureblock
name: Corrosive Pool
type: Hazard Hexer
level: 2
ev: 3 per 10 x 10 pool
flavor: This shallow pool bubbles with acid or some other corrosive liquid.
stamina: 12 per square
size: One or more squares of difficult terrain
stats:
  - name: Immunity
    value: 20 to all damage except cold or fire damage
features:
  - name: Deactivate
    icon: 🌀
    effects:
      - effect: The pool must be completely destroyed.
  - name: Activate
    icon: ❕
    effects:
      - effect: A creature or object enters the corrosive pool or starts their turn
          there. The liquid in the pool is also highly volatile (see **Explosive
          Reaction** below).
      - effect: A creature or object takes 3 acid damage if they start their turn in the
          pool, and takes 3 acid damage for each square of the pool they enter.
        name: Effect
  - name: Explosive Reaction
    icon: ❗️
    keywords:
      - Area
    type: Free triggered action
    distance: 3 burst
    target: Each creature and object in the area
    trigger: The pool takes fire damage.
    effects:
      - roll: Power Roll + 2
        t1: 3 fire damage; M < 1 the target is burning (save ends)
        t2: 6 fire damage; M < 2 the target is burning (save ends)
        t3: 9 fire damage; M < 3 the target is burning (save ends)
      - effect: The liquid in the pool is consumed. This ability has a double edge
          against any target in the pool. A burning creature takes 1d6 fire
          damage at the start of each of their turns. A burning object takes 1d6
          fire damage at the end of each round. Any target with acid weakness
          takes extra damage from this ability and while burning as if the fire
          damage were acid damage.
        name: Effect
  - name: Allied Awareness
    icon: ⭐️
    effects:
      - effect: Allies who have weapons are equipped with torches. Any ally can use a
          maneuver to throw a torch up to 5 squares and deal 1 fire damage to
          the pool, triggering Explosive Reaction.
~~~