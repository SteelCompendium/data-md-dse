---
file_basename: Watchtower
file_dpath: Dynamic Terrain/Siege Engines
item_id: watchtower-level-2-fortification-defender
item_index: '04'
item_name: Watchtower (Level 2 Fortification Defender)
scc:
- mcdm.monsters.v1:dynamic-terrain.siege-engine:watchtower-level-2-fortification-defender
scdc:
- 1.1.1:4.2:04
source: mcdm.monsters.v1
type: dynamic-terrain/siege-engine
---

~~~ds-featureblock
type: featureblock
featureblock_type: Fortification Defender
name: Watchtower
level: 2
ev: "8"
flavor: A sturdy wooden tower accessed by interior ladders or stairs provides
  cover and high ground for attackers.
stamina: "50"
size: "3"
features:
  - type: feature
    feature_type: trait
    name: Deactivate
    icon: 🌀
    effects:
      - effect: The watchtower must be completely destroyed.
  - type: feature
    feature_type: trait
    name: High Ground and Cover
    icon: ⭐️
    effects:
      - effect: Creatures who have access to the watchtower's interior ladders or stairs
          have high ground and cover against creatures outside the watchtower.
  - type: feature
    feature_type: trait
    name: Getting Inside
    icon: 🌀
    effects:
      - effect: A creature outside and adjacent to the watchtower can gain access to the
          interior by climbing it as an **Agility test** or breaking into it
          with a **Might test**.
        tier1: 1d6 damage; the creature remains outside the watchtower
        tier2: The creature remains outside the watchtower.
        tier3: The creature gains access to the watchtower.
  - type: feature
    feature_type: trait
    name: Upgrades
    icon: ⭐️
    effects:
      - name: Ballista Emplacement
        cost: +12 EV
        effect: The watchtower is equipped with a field ballista that can be used by
          creatures in the watchtower. The ballista can't be moved.
      - name: Boiling Oil Cauldron
        cost: +17 EV
        effect: The watchtower is equipped with a boiling oil cauldron that can be used
          by creatures in the watchtower.
      - name: Spyglass
        cost: +2 EV
        effect: Any creature in the watchtower can use the spyglass to search for hidden
          creatures around the tower, gaining an edge on the Intuition test and
          increasing the distance at which creatures can be spotted to 15
          squares.
      - name: Stone Tower
        cost: +2 EV
        effect: The watchtower is reinforced with stone and has 75 Stamina.
      - name: Iron Tower
        cost: +4 EV
        effect: The watchtower is reinforced with stone and iron and has 100 Stamina.
~~~