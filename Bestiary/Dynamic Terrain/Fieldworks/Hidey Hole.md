---
file_basename: Hidey Hole
file_dpath: Dynamic Terrain/Fieldworks
item_id: hidey-hole-level-1-fortification-ambusher
item_index: '04'
item_name: Hidey-Hole (Level 1 Fortification Ambusher)
scc:
- mcdm.monsters.v1:dynamic-terrain.fieldwork:hidey-hole-level-1-fortification-ambusher
scdc:
- 1.1.1:4.3:04
source: mcdm.monsters.v1
type: dynamic-terrain/fieldwork
---

~~~ds-featureblock
name: Hidey-Hole
type: Fortification Ambusher
level: 1
ev: "1"
flavor: A cavity in a floor, wall, or ceiling might hold hidden threats.
stamina: "-"
size: One or more squares
features:
  - name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to a hidey-hole can make a **Might
          test**.
        t1: The creature is restrained (save ends).
        t2: The hidey-hole collapses but the creature is slowed (save ends).
        t3: The hidey-hole collapses and can no longer be used until repaired.
  - name: Activate
    icon: ❕
    effects:
      - effect: A creature starts the encounter in the hidey-hole or ends their turn
          there.
      - effect: The triggering creature can attempt to hide as a free triggered action.
        name: Effect
  - name: Upgrade
    icon: ⭐️
    effects:
      - effect: "**Network (+1 EV per hidey-hole)** The hidey-hole is connected to a
          tunnel network. A creature familiar with the network can move from one
          hidey-hole to any space adjacent to a connected hidey-hole if they
          have movement available equal to the straight-line distance to that
          space. A creature unfamiliar with the network can use a maneuver to
          make a **hard Intuition test** to discover a connected hidey-hole."
~~~