---
file_basename: Toxic Plants
file_dpath: Dynamic Terrain/Environmental Hazards
item_id: toxic-plants-level-2-hazard-hexer
item_index: '05'
item_name: Toxic Plants (Level 2 Hazard Hexer)
scc:
- mcdm.monsters.v1:dynamic-terrain.environmental-hazard:toxic-plants-level-2-hazard-hexer
scdc:
- 1.1.1:4.5:05
source: mcdm.monsters.v1
type: dynamic-terrain/environmental-hazard
---

~~~ds-featureblock
name: Toxic Plants
type: Hazard Hexer
level: 2
ev: 2 per 10 x 10 field
flavor: Colorful mushrooms or lovely flowering plants release a cloud of spores
  or pollen when disturbed, causing creatures to fall into a magical slumber.
stamina: 3 per square
size: One or more squares
stats: []
features:
  - name: Deactivate
    icon: 🌀
    effects:
      - effect: Each square of plants must be individually destroyed.
  - name: Activate
    icon: ❕
    effects:
      - effect: A creature starts their turn in the area of the toxic plants, or enters
          a square of toxic plants without shifting.
      - effect: The **Sleep Spores** ability.
        name: Effect
  - name: Sleep Spores
    icon: ❗️
    keywords:
      - Magic
      - Melee
      - Strike
    type: Free triggered action
    distance: Melee 0
    target: The triggering creature
    trigger: A creature starts their turn in the area of the toxic plants, or enters
      a square of toxic plants without shifting.
    effects:
      - effect: Magic, Melee, Strike Free triggered action
      - roll: Power Roll + 2
        t1: M < 0 dazed (save ends)
        t2: M < 1 dazed (save ends)
        t3: M < 2 dazed (save ends)
      - effect: While dazed this way, a target who starts their turn in the area of the
          toxic plants falls prone and can't stand.
        name: Effect
  - name: Upgrades
    icon: ⭐️
    effects:
      - effect: "**Poisonous Spores (+2 EV)** Any creature dazed by this hazard takes
          1d6 poison damage at the start of each of their turns."
      - effect: "**Carnivorous Plants (+2 EV)** The plants are carnivorous and attempt
          to slowly digest any creature who falls among them. Any creature who
          starts their turn prone in the area takes 4 acid damage."
~~~