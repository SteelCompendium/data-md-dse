---
file_basename: Spike Trap
file_dpath: Dynamic Terrain/Fieldworks
item_id: spike-trap-level-2-trap-ambusher
item_index: '06'
item_name: Spike Trap (Level 2 Trap Ambusher)
scc:
- mcdm.monsters.v1:dynamic-terrain.fieldwork:spike-trap-level-2-trap-ambusher
scdc:
- 1.1.1:4.3:06
source: mcdm.monsters.v1
type: dynamic-terrain/fieldwork
---

~~~ds-featureblock
name: Spike Trap
type: Trap Ambusher
level: 2
ev: "3"
flavor: A pit dug into the ground is filled with spikes, and camouflaged to
  avoid detection.
stamina: "6"
size: One or more squares
stats:
  - name: Typical Space
    value: 2 x 2-square area
features:
  - name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to a spike trap can make an **Agility
          test**.
        t1: The creature triggers the trap and is affected as if in its area.
        t2: The trap is deactivated but the creature is slowed (EoT).
        t3: The trap is deactivated and doesn't trigger.
  - name: Activate
    icon: ❕
    effects:
      - effect: The spike trap is calibrated to be triggered by creatures or objects of
          a particular size or larger. The trap triggers when a creature or
          object of the appropriate size enters its area.
      - effect: The **Spike Trap** ability.
        name: Effect
  - name: Spike Trap
    icon: ❗️
    keywords:
      - Area
      - Weapon
    type: Free triggered action
    distance: Melee 0
    target: The triggering creature or object
    trigger: A creature or object of the appropriate size enters the trap's area.
    effects:
      - roll: Power Roll + 2
        t1: 3 damage; the target shifts 1 square away from the trap
        t2: 4 damage; the target falls into the pit; A < 0 prone
        t3: 6 damage; the target falls into the pit; A < 1 prone; restrained (save ends)
      - effect: The target ends their movement when they enter the trap's area. The pit
          is typically 2 squares deep. The trap must be manually reset.
        name: Effect
  - name: Hidden
    icon: ⭐️
    effects:
      - effect: The spike trap is hidden until triggered or detected.
~~~