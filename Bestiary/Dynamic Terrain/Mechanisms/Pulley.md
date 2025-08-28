---
file_basename: Pulley
file_dpath: Dynamic Terrain/Mechanisms
item_id: pulley-level-1-trigger-support
item_index: 08
item_name: Pulley (Level 1 Trigger Support)
scc:
- mcdm.monsters.v1:dynamic-terrain.mechanism:pulley-level-1-trigger-support
scdc:
- 1.1.1:4.1:08
source: mcdm.monsters.v1
type: dynamic-terrain/mechanism
---

~~~ds-featureblock
name: Pulley
type: Trigger Support
level: 1
ev: "1"
flavor: A counterweighted pulley system can be used to quickly ascend to the top
  of a wall, scaffold, tower, or other structure.
stamina: "1"
size: 1S
stats: []
features:
  - name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to a pulley can make an **Agility
          test**.
        t1: The creature triggers the pulley.
        t2: The pulley is deactivated but the creature is slowed (EoT).
        t3: The pulley is deactivated and doesn't trigger.
  - name: Activate
    icon: ❕
    effects:
      - effect: A creature adjacent to the pulley uses a maneuver to release the pulley.
      - effect: The triggering creature is lifted to the top of the structure the pulley
          is attached to. The pulley must be manually reset.
        name: Effect
  - name: Climbable
    icon: ⭐️
    effects:
      - effect: A creature adjacent to the pulley can climb its ropes with an **easy
          Agility test** to ascend to the top of the structure it's attached to.
  - name: Upgrade
    icon: ⭐️
    effects:
      - effect: "**Looped Chain (+1 EV)** Instead of a rope and pulley, the system uses
          a counterweighted looped chain. A looped chain automatically resets
          and can be triggered repeatedly."
~~~