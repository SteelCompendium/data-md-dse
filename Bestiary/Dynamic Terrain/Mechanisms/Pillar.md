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
name: Pillar
type: Hazard Hexer
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
  - name: Deactivate
    icon: 🌀
    effects:
      - effect: The pillar's linked trigger must be deactivated.
  - name: Activate
    icon: ❕
    effects:
      - effect: The pillar is destroyed, or a pressure plate, switch, or other linked
          trigger is activated.
      - effect: The **Toppling Pillar** ability.
        name: Effect
  - name: Toppling Pillar
    icon: ❗️
    keywords:
      - Area
    type: Free triggered action
    distance: 4 x 1 line within 1
    target: Each creature and object in the area
    trigger: The pillar is destroyed, or a pressure plate, switch, or other linked
      trigger is activated.
    effects:
      - roll: Power Roll + 2
        t1: 4 damage
        t2: 6 damage; M < 1 restrained (save ends)
        t3: 9 damage; M < 2 restrained (save ends)
      - effect: The area is difficult terrain.
        name: Effect
  - name: Upgrades
    icon: ⭐️
    effects:
      - effect: "**Metal Pillar (+1 EV)** The pillar is made of metal, has 9 Stamina,
          and deals 1d6 extra damage."
      - effect: "**Multiple Pillars (+3 EV per additional pillar)** Multiple pillars can
          be used to represent a larger toppling object such as a wall. If
          triggered by destruction, all individual pillars need to be destroyed
          before the object falls."
~~~