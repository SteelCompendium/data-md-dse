---
file_basename: Dart Trap
file_dpath: Dynamic Terrain/Mechanisms
item_id: dart-trap-level-1-trap-ambusher
item_index: '02'
item_name: Dart Trap (Level 1 Trap Ambusher)
scc:
- mcdm.monsters.v1:dynamic-terrain.mechanism:dart-trap-level-1-trap-ambusher
scdc:
- 1.1.1:4.1:02
source: mcdm.monsters.v1
type: dynamic-terrain/mechanism
---

~~~ds-featureblock
name: Dart Trap
type: Trap Ambusher
level: 1
ev: "1"
flavor: A concealed dart thrower hurls missiles at short range.
stamina: "3"
size: 1S
stats:
  - name: Direction
    value: The dart trap fires in a fixed direction.
features:
  - name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to a dart trap can make an **Agility
          test**.
        t1: The creature triggers the trap and is targeted by it.
        t2: The trap is deactivated but the creature is slowed (EoT).
        t3: The trap is deactivated and doesn't trigger.
  - name: Activate
    icon: ❕
    effects:
      - effect: A pressure plate, switch, or other linked trigger is activated.
      - effect: The **Dart** ability.
        name: Effect
  - name: Dart
    icon: ❗️
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Free triggered action
    distance: Ranged 5
    target: One creature or object
    trigger: A pressure plate, switch, or other linked trigger is activated.
    effects:
      - roll: Power Roll + 2
        t1: 2 damage
        t2: 4 damage
        t3: 5 damage
  - name: Upgrades
    icon: ⭐️
    effects:
      - effect: The darts are tipped with poison. Any creature who takes damage from a
          dart also takes 1d6 poison damage at the start of each of their turns
          (save ends).
        name: Poison Darts
        cost: +2 EV
      - effect: Larger, heavier darts impart kinetic force to the trap's attack. A
          target of the **Dart** ability is pushed 1 square on a tier 1 outcome,
          2 squares on a tier 2 outcome, or 3 squares on a tier 3 outcome.
        name: Large Darts
        cost: +1 EV
      - effect: The dart trap is equipped with multiple barrels to launch darts at a
          high rate of fire. The **Dart** ability loses the Ranged and Strike
          and takes the Area keyword, its area becomes a 5 x 1 line within 1,
          and it deals an extra 1d6 damage.
        name: Gatling Darts
        cost: +4 EV
  - name: Hidden
    icon: ⭐️
    effects:
      - effect: The dart trap is hidden until triggered or detected.
~~~