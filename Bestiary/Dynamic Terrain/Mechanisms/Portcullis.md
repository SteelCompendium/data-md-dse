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
name: Portcullis
type: Trap Ambusher
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
  - name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to a portcullis can make an **Agility
          test**.
        t1: The creature triggers the portcullis and is affected as if in its area.
        t2: The portcullis is deactivated but the creature is slowed (EoT).
        t3: The portcullis is deactivated and doesn't trigger.
  - name: Activate
    icon: ❕
    effects:
      - effect: A pressure plate, switch, or other linked trigger is activated.
      - effect: The **Heavy Gate** ability.
        name: Effect
  - name: Heavy Gate
    icon: ❗️
    keywords:
      - Area
      - Weapon
    type: Free triggered action
    distance: Special
    target: Each creature and object in the area
    trigger: A pressure plate, switch, or other linked trigger is activated.
    effects:
      - name: Special
        effect: The area of this ability is the area directly beneath the portcullis
          when it falls.
      - roll: Power Roll + 2
        t1: 3 damage; slide 1, ignoring stability
        t2: 7 damage; A < 2 restrained (save ends)
        t3: 10 damage; A < 3 restrained (save ends)
      - effect: The portcullis blocks movement from one side of it to the other. A
          target slid by the portcullis ends up on one side of it or the other
          (choose randomly). The portcullis must be manually reset.
        name: Effect
  - name: Hidden
    icon: ⭐️
    effects:
      - effect: The portcullis is hidden until triggered or detected.
~~~