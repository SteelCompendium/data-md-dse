---
file_basename: Bear Trap
file_dpath: Dynamic Terrain/Fieldworks
item_id: bear-trap-level-1-trap-ambusher
item_index: '05'
item_name: Bear Trap (Level 1 Trap Ambusher)
scc:
- mcdm.monsters.v1:dynamic-terrain.fieldwork:bear-trap-level-1-trap-ambusher
scdc:
- 1.1.1:4.3:05
source: mcdm.monsters.v1
type: dynamic-terrain/fieldwork
---

~~~ds-featureblock
name: Bear Trap
type: Trap Ambusher
level: 1
ev: "2"
flavor: A set of spring-loaded steel jaws stands ready to snap shut when stepped on.
stamina: "6"
size: 1S
features:
  - name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to a bear trap can make an **Agility
          test**.
        t1: The creature triggers the trap and is affected as if in its space.
        t2: The trap is deactivated but the creature is slowed (EoT).
        t3: The trap is deactivated and doesn't trigger.
  - name: Activate
    icon: ❕
    effects:
      - effect: The bear trap is calibrated to be triggered by creatures or objects of a
          particular size or larger. The trap triggers when a creature or object
          of the appropriate size enters its space.
      - effect: A triggering creature or object ends their movement and is targeted by
          the **Bear Trap** ability.
        name: Effect
  - name: Bear Trap
    icon: ❗️
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Free triggered action
    distance: Melee 0
    target: The triggering creature or object
    trigger: A creature or object of the appropriate size enters the trap's space.
    effects:
      - roll: Power Roll + 2
        t1: 1 The target shifts 1 square away from the trap.
        t2: 3 damage; A < 1 slowed (save ends)
        t3: 5 damage; A < 2 slowed (save ends)
      - effect: The bear trap must be manually reset.
        name: Effect
  - name: Upgrade
    icon: ⭐️
    effects:
      - effect: The bear trap is attached to the ground by a steel chain. A target who
          would be made slowed by the trap is restrained instead.
        name: Chain
        cost: +1 EV
  - name: Hidden
    icon: ⭐️
    effects:
      - effect: The bear trap is hidden until triggered or detected.
~~~