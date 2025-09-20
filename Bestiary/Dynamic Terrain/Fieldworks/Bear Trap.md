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
type: featureblock
featureblock_type: Trap Ambusher
name: Bear Trap
level: 1
ev: "2"
flavor: A set of spring-loaded steel jaws stands ready to snap shut when stepped on.
stamina: "6"
size: 1S
features:
  - type: feature
    feature_type: trait
    name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to a bear trap can make an **Agility
          test**.
        tier1: The creature triggers the trap and is affected as if in its space.
        tier2: The trap is deactivated but the creature is slowed (EoT).
        tier3: The trap is deactivated and doesn't trigger.
  - type: feature
    feature_type: trait
    name: Activate
    icon: ❕
    effects:
      - effect: The bear trap is calibrated to be triggered by creatures or objects of a
          particular size or larger. The trap triggers when a creature or object
          of the appropriate size enters its space.
      - name: Effect
        effect: A triggering creature or object ends their movement and is targeted by
          the **Bear Trap** ability.
  - type: feature
    feature_type: ability
    name: Bear Trap
    icon: ❗️
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Free triggered action
    distance: Melee 0
    target: The triggering creature or object
    trigger: A creature or object of the appropriate size enters the trap's space.
    effects:
      - roll: Power Roll + 2
        tier1: 1 The target shifts 1 square away from the trap.
        tier2: 3 damage; A < 1 slowed (save ends)
        tier3: 5 damage; A < 2 slowed (save ends)
      - name: Effect
        effect: The bear trap must be manually reset.
  - type: feature
    feature_type: trait
    name: Upgrade
    icon: ⭐️
    effects:
      - name: Chain
        cost: +1 EV
        effect: The bear trap is attached to the ground by a steel chain. A target who
          would be made slowed by the trap is restrained instead.
  - type: feature
    feature_type: trait
    name: Hidden
    icon: ⭐️
    effects:
      - effect: The bear trap is hidden until triggered or detected.
~~~