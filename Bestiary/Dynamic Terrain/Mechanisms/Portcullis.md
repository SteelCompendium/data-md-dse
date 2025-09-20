---
file_basename: Portcullis
file_dpath: Dynamic Terrain/Mechanisms
item_id: portcullis-level-3-trap-ambusher
item_index: '06'
item_name: Portcullis (Level 3 Trap Ambusher)
scc:
- mcdm.monsters.v1:dynamic-terrain.mechanism:portcullis-level-3-trap-ambusher
scdc:
- 1.1.1:4.1:06
source: mcdm.monsters.v1
type: dynamic-terrain/mechanism
---

~~~ds-featureblock
type: featureblock
featureblock_type: Trap Ambusher
name: Portcullis
level: 3
ev: "4"
flavor: A portcullis is hidden in the ceiling of a passage or choke point,
  waiting to drop when activated.
stamina: 9 per square
size: The area of the corridor to be blocked
stats:
  - name: Typical Space
    value: 2 x 1-square area, up to a 4 x 2-square area
features:
  - type: feature
    feature_type: trait
    name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to a portcullis can make an **Agility
          test**.
        tier1: The creature triggers the portcullis and is affected as if in its area.
        tier2: The portcullis is deactivated but the creature is slowed (EoT).
        tier3: The portcullis is deactivated and doesn't trigger.
  - type: feature
    feature_type: trait
    name: Activate
    icon: ❕
    effects:
      - effect: A pressure plate, switch, or other linked trigger is activated.
      - name: Effect
        effect: The **Heavy Gate** ability.
  - type: feature
    feature_type: ability
    name: Heavy Gate
    icon: ❗️
    keywords:
      - Area
      - Weapon
    usage: Free triggered action
    distance: Special
    target: Each creature and object in the area
    trigger: A pressure plate, switch, or other linked trigger is activated.
    effects:
      - name: Special
        effect: The area of this ability is the area directly beneath the portcullis
          when it falls.
      - roll: Power Roll + 2
        tier1: 3 damage; slide 1, ignoring stability
        tier2: 7 damage; A < 2 restrained (save ends)
        tier3: 10 damage; A < 3 restrained (save ends)
      - name: Effect
        effect: The portcullis blocks movement from one side of it to the other. A
          target slid by the portcullis ends up on one side of it or the other
          (choose randomly). The portcullis must be manually reset.
  - type: feature
    feature_type: trait
    name: Hidden
    icon: ⭐️
    effects:
      - effect: The portcullis is hidden until triggered or detected.
~~~