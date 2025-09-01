---
file_basename: The Black Obelisk
file_dpath: Dynamic Terrain/Supernatural Objects
item_id: the-black-obelisk-level-3-relic-controller
item_index: '01'
item_name: The Black Obelisk (Level 3 Relic Controller)
scc:
- mcdm.monsters.v1:dynamic-terrain.supernatural-object:the-black-obelisk-level-3-relic-controller
scdc:
- 1.1.1:4.6:01
source: mcdm.monsters.v1
type: dynamic-terrain/supernatural-object
---

~~~ds-featureblock
name: The Black Obelisk
type: Relic Controller
level: 3
ev: "20"
flavor: A foreboding obelisk shaped of dark stone harrows the minds and spirits
  of those around it.
stamina: "100"
size: "2"
features:
  - name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to the black obelisk can make a
          **Reason test**.
        t1: The creature accidentally activates the **Your Fears Become Manifest**
          ability, which gains an edge.
        t2: The creature must make another test to deactivate the obelisk. If they
          obtain this outcome a second time, they accidentally activate **Your
          Fears Become Manifest**.
        t3: The obelisk is deactivated until the end of the encounter.
  - name: Activate
    icon: ❕
    effects:
      - effect: A new round starts.
      - effect: The **Your Fears Become Manifest** ability.
        name: Effect
  - name: Your Fears Become Manifest
    icon: ❗️
    keywords:
      - Area
      - Magic
    type: Free triggered action
    distance: 10 burst
    target: Each enemy in the area
    trigger: A new round starts.
    effects:
      - roll: Power Roll + 2
        t1: P < 1 slowed (EoT)
        t2: P < 2 slowed and weakened (EoT)
        t3: P < 3 frightened, slowed, and weakened (EoT)
      - effect: The target is pushed 2 squares.
        name: Effect
~~~