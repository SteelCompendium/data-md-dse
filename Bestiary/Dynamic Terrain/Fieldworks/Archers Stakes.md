---
file_basename: Archers Stakes
file_dpath: Dynamic Terrain/Fieldworks
item_id: archers-stakes-level-1-fortification-defender
item_index: '02'
item_name: Archer's Stakes (Level 1 Fortification Defender)
scc:
- mcdm.monsters.v1:dynamic-terrain.fieldwork:archers-stakes-level-1-fortification-defender
scdc:
- 1.1.1:4.3:02
source: mcdm.monsters.v1
type: dynamic-terrain/fieldwork
---

~~~ds-featureblock
type: featureblock
featureblock_type: Fortification Defender
name: Archer's Stakes
level: 1
ev: "2"
flavor: A series of sharp stakes have been placed point-out to protect defenders
  against charges and other direct attacks.
stamina: 3 per square
size: One or more squares of difficult terrain
stats:
  - name: Typical Space
    value: 4 x 1-square area
  - name: Direction
    value: One side of the stakes is defined as the front.
features:
  - type: feature
    feature_type: trait
    name: Deactivate
    icon: 🌀
    effects:
      - effect: Each square of stakes must be individually destroyed.
  - type: feature
    feature_type: trait
    name: Activate
    icon: ❕
    effects:
      - effect: A creature enters an area of stakes from the front.
      - name: Effect
        effect: The triggering creature takes 2 damage per square of stakes they enter.
          If they are force moved into an area of stakes, they take an
          additional 3 damage.
  - type: feature
    feature_type: trait
    name: Upgrades
    icon: ⭐️
    effects:
      - name: Poison
        cost: +2 EV
        effect: The tips of the stakes have poison applied to them. Any creature who
          takes damage from the stakes also takes 1d6 poison damage at the start
          of each of their turns (save ends).
      - name: Sticky
        cost: +3 EV
        effect: A sticky slime or webbing has been applied to the stakes and the ground
          between them. Any creature who enters an area of stakes triggers the
          **Sticky Stakes** ability in addition to suffering the stakes' other
          effects.
  - type: feature
    feature_type: ability
    name: Sticky Stakes
    icon: ❗️
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Free triggered action
    distance: Melee 0
    target: The triggering creature or object
    trigger: A creature or object enters an area of sticky stakes.
    effects:
      - roll: Power Roll + 2
        tier1: No effect.
        tier2: A < 1 slowed (save ends)
        tier3: A < 2 restrained (save ends)
  - type: feature
    feature_type: trait
    name: Allied Awareness
    icon: ⭐️
    effects:
      - effect: Allies of this object ignore the difficult terrain created by the
          stakes, take no damage from moving through the stakes unless they are
          force moved, and have cover while in an area of archer's stakes.
~~~