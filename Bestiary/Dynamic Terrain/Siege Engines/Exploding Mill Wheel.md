---
file_basename: Exploding Mill Wheel
file_dpath: Dynamic Terrain/Siege Engines
item_id: exploding-mill-wheel-level-3-siege-engine-artillery
item_index: '05'
item_name: Exploding Mill Wheel (Level 3 Siege Engine Artillery)
scc:
- mcdm.monsters.v1:dynamic-terrain.siege-engine:exploding-mill-wheel-level-3-siege-engine-artillery
scdc:
- 1.1.1:4.2:05
source: mcdm.monsters.v1
type: dynamic-terrain/siege-engine
---

~~~ds-featureblock
name: Exploding Mill Wheel
type: Siege Engine Artillery
level: 3
ev: "10"
flavor: A massive wooden wheel is loaded with explosives and rolled toward enemy
  forces or fortifications, ready to explode.
stamina: "25"
size: "2"
features:
  - name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to an exploding mill wheel that isn't
          rolling can make an **Agility test**.
        t1: The creature accidentally activates the **Roll the Wheel** ability.
        t2: The exploding mill wheel is deactivated but the creature is slowed (EoT).
        t3: The exploding mill wheel is deactivated and can't be used.
      - effect: Once the wheel is rolling, it can't be deactivated. However, it can be
          exploded early by destroying it or blocking its movement with a
          suitably large creature or object.
  - name: Roll the Wheel
    icon: 🌀
    keywords:
      - Area
    type: Main action (Adjacent creature)
    distance: Special
    target: Each creature and object in the area
    effects:
      - name: Effect
        effect: When this ability is used and at the start of every turn thereafter, the
          exploding mill wheel rolls, moving 2 squares in a straight line. Each
          creature and object of size 2 or smaller in the area defined by the
          wheel's movement is targeted by the following power roll. A target
          force moved this way is moved to either side of the wheel, as the
          Director determines.
      - roll: Power Roll + 2
        t1: 5 damage; push 1
        t2: 9 damage; push 2
        t3: 12 damage; push 3
      - effect: If the wheel enters the space of any creature or object of size 3 or
          larger, or if it is reduced to 0 Stamina, its movement stops and it
          explodes. Each creature and object in a 5 burst centered on the wheel
          is targeted by the following power roll.
        t1: 5 damage; push 1; M < 0 burning (save ends)
        t2: 9 damage; push 2; M < 1 burning (save ends)
        t3: 12 damage; push 3; M < 2 burning (save ends)
      - effect: A burning creature takes 1d6 fire damage at the start of each of their
          turns. A burning object takes 1d6 fire damage at the end of each
          round.
  - name: Upgrade
    icon: ⭐️
    effects:
      - name: Piloted
        cost: +4 EV
        effect: >-
          The wheel has been fitted with a control mechanism and a pilot's seat
          for a creature of size 1M or smaller. As a move action, the pilot can
          turn the wheel in any direction while it is moving. As a main action,
          the pilot can leap out of the pilot's seat, landing in an adjacent
          space while the wheel continues moving in a straight line.

          Without proper training, determining how to pilot the wheel requires a
          **Reason test**.
        t1: The wheel immediately explodes as if striking a size 3 or larger creature or
          object.
        t2: The creature fails to pilot the wheel.
        t3: The creature can pilot the wheel.
      - effect: On a natural 19 or 20, a creature can both pilot the wheel and can
          disarm its explosives as a maneuver.
~~~