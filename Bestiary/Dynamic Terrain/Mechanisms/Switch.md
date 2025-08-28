---
file_basename: Switch
file_dpath: Dynamic Terrain/Mechanisms
item_id: switch-level-1-trigger-support
item_index: '07'
item_name: Switch (Level 1 Trigger Support)
scc:
- mcdm.monsters.v1:dynamic-terrain.mechanism:switch-level-1-trigger-support
scdc:
- 1.1.1:4.1:07
source: mcdm.monsters.v1
type: dynamic-terrain/mechanism
---

~~~ds-featureblock
name: Switch
type: Trigger Support
level: 1
ev: "1"
flavor: Set into any surface, this mechanism acts as a trigger for another
  linked mechanism.
stamina: "3"
size: 1T
stats:
  - name: Link
    value: A switch is linked to another mechanism that it activates when triggered.
features:
  - name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to a switch can make an **Agility
          test**.
        t1: The creature triggers the switch.
        t2: The switch is deactivated but the creature is slowed (EoT).
        t3: The switch is deactivated and doesn't trigger.
  - name: Activate
    icon: ❕
    effects:
      - effect: A creature adjacent to the switch uses a maneuver to trigger it.
      - effect: The linked mechanism is activated. A switch automatically resets and can
          be triggered repeatedly.
        name: Effect
  - name: Upgrade
    icon: ⭐️
    effects:
      - effect: "**Concealed (+1 EV)** The switch is hidden."
~~~