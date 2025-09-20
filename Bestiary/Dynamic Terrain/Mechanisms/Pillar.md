---
file_basename: Pillar
file_dpath: Dynamic Terrain/Mechanisms
item_id: pillar-level-2-hazard-hexer
item_index: '05'
item_name: Pillar (Level 2 Hazard Hexer)
scc:
- mcdm.monsters.v1:dynamic-terrain.mechanism:pillar-level-2-hazard-hexer
scdc:
- 1.1.1:4.1:05
source: mcdm.monsters.v1
type: dynamic-terrain/mechanism
---

~~~ds-featureblock
type: featureblock
featureblock_type: Hazard Hexer
name: Pillar
level: 2
ev: "3"
flavor: This stone pillar can be toppled onto unsuspecting foes with the right
  amount of damage or a well-engineered trigger mechanism.
stamina: "6"
size: One square that can't be moved through
stats:
  - name: Direction
    value: The pillar topples in a preset direction.
features:
  - type: feature
    feature_type: trait
    name: Deactivate
    icon: 🌀
    effects:
      - effect: The pillar's linked trigger must be deactivated.
  - type: feature
    feature_type: trait
    name: Activate
    icon: ❕
    effects:
      - effect: The pillar is destroyed, or a pressure plate, switch, or other linked
          trigger is activated.
      - name: Effect
        effect: The **Toppling Pillar** ability.
  - type: feature
    feature_type: ability
    name: Toppling Pillar
    icon: ❗️
    keywords:
      - Area
    usage: Free triggered action
    distance: 4 x 1 line within 1
    target: Each creature and object in the area
    trigger: The pillar is destroyed, or a pressure plate, switch, or other linked
      trigger is activated.
    effects:
      - roll: Power Roll + 2
        tier1: 4 damage
        tier2: 6 damage; M < 1 restrained (save ends)
        tier3: 9 damage; M < 2 restrained (save ends)
      - name: Effect
        effect: The area is difficult terrain.
  - type: feature
    feature_type: trait
    name: Upgrades
    icon: ⭐️
    effects:
      - name: Metal Pillar
        cost: +1 EV
        effect: The pillar is made of metal, has 9 Stamina, and deals 1d6 extra damage.
      - name: Multiple Pillars
        cost: +3 EV per additional pillar
        effect: Multiple pillars can be used to represent a larger toppling object such
          as a wall. If triggered by destruction, all individual pillars need to
          be destroyed before the object falls.
~~~