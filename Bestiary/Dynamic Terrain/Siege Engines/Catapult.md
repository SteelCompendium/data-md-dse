---
file_basename: Catapult
file_dpath: Dynamic Terrain/Siege Engines
item_id: catapult-level-3-siege-engine-artillery
item_index: '07'
item_name: Catapult (Level 3 Siege Engine Artillery)
scc:
- mcdm.monsters.v1:dynamic-terrain.siege-engine:catapult-level-3-siege-engine-artillery
scdc:
- 1.1.1:4.2:07
source: mcdm.monsters.v1
type: dynamic-terrain/siege-engine
---

~~~ds-featureblock
name: Catapult
type: Siege Engine Artillery
level: 3
ev: "10"
flavor: This massive counterweighted engine hurls a heavy projectile for a
  devastating assault.
stamina: "50"
size: "2"
features:
  - name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to a catapult can make an **Agility
          test**.
        t1: The creature accidentally activates the **Arcing Shot** ability.
        t2: The catapult is deactivated but the creature is slowed (EoT).
        t3: The catapult is deactivated and can't be used.
  - name: Arcing Shot
    icon: 🔳
    keywords:
      - "- Area"
      - Ranged
      - Weapon
    type: Main action (Adjacent creature)
    distance: 3 cube within 20
    target: Each creature and object in the area
    effects:
      - roll: Power Roll + 2
        t1: 5 damage
        t2: 9 damage; A < 0 push 1
        t3: 12 damage; A < 1 push 2
      - effect: Line of effect for this ability is an arc that can be traced over
          obstacles between the catapult and the target area. This ability can't
          be used again until the catapult is reloaded.
        name: Effect
  - name: Reload
    icon: ⭐️
    keywords:
      - "-"
    type: Main action (Adjacent creature)
    distance: "-"
    target: "-"
    effects:
      - effect: The catapult is reloaded, allowing **Arcing Shot** to be used again.
          This action can be used only once per round.
        name: Effect
  - name: Spot
    icon: ⭐️
    keywords:
      - "-"
    type: Main action (Adjacent creature)
    distance: "-"
    target: "-"
    effects:
      - effect: The next use of **Arcing Shot** gains an edge and has a +10 bonus to
          ranged distance. This action can be used only once per round.
        name: Effect
  - name: Move
    icon: ⭐️
    keywords:
      - "-"
    type: Main action (Adjacent creature)
    distance: "-"
    target: "-"
    effects:
      - effect: The catapult and the creature using this action move together up to 2
          squares.
        name: Effect
  - name: Upgrades
    icon: ⭐️
    effects:
      - effect: The side fielding the catapult has trained their forces to safely use
          the siege engine to launch them across the battlefield. As an adjacent
          creature main action, the catapult can be used to vertical push 10 any
          ally of size 1L or less. If the ally lands in an unoccupied space,
          they take no damage.
        name: Air Assault
        cost: +2 EV
      - effect: deals fire damage, and the area of that ability is on fire until the end
          of the encounter. Any creature who enters the area for the first time
          in a round or starts their turn there takes 2 fire damage.
        name: Flammable
        cost: +2 EV
~~~