---
file_basename: Ram
file_dpath: Dynamic Terrain/Mechanisms
item_id: ram-level-2-trap-ambusher
item_index: '01'
item_name: Ram (Level 2 Trap Ambusher)
scc:
- mcdm.monsters.v1:dynamic-terrain.mechanism:ram-level-2-trap-ambusher
scdc:
- 1.1.1:4.1:01
source: mcdm.monsters.v1
type: dynamic-terrain/mechanism
---

~~~ds-featureblock
name: Ram
type: Trap Ambusher
level: 2
ev: "3"
flavor: A heavy wooden ram drops down or swings into the fray, crushing all in
  its path.
stamina: 3 per square
size: Any area; the area can't be moved through
stats:
  - name: Typical Space
    value: 1 x 3-square area or a 2 x 2-square area
  - name: Direction
    value: One side of the ram is defined as the front.
features:
  - name: Deactivate
    icon: 🌀
    effects:
      - effect: As a maneuver, a creature adjacent to a ram can make an **Agility
          test**.
        t1: The creature triggers the ram and is affected as if in its space.
        t2: The ram is deactivated but the creature is slowed (EoT).
        t3: The ram is deactivated and doesn't trigger.
  - name: Activate
    icon: ❕
    effects:
      - effect: A pressure plate, switch, or other linked trigger is activated.
      - effect: The **Ram** ability.
        name: Effect
  - name: Ram
    icon: ❗️
    keywords:
      - Area
      - Weapon
    type: Free triggered action
    distance: Special
    target: Each creature and object in the area
    trigger: A pressure plate, switch, or other linked trigger is activated.
    effects:
      - name: Special
        effect: The area of this ability is the path the ram moves through from its
          starting position.
      - roll: Power Roll + 2
        t1: 3 damage; slide 1, ignoring stability
        t2: 6 damage; push 3
        t3: 9 damage; push 5
      - effect: A target slid by the ram ends up on one side of it or the other (choose
          randomly). The ram must be manually reset.
        name: Effect
  - name: Upgrades
    icon: ⭐️
    effects:
      - effect: The ram is made of stone, has 6 Stamina per square, and deals an extra
          1d3 damage.
        name: Stone
        cost: +1 EV
      - effect: The ram is made of metal, has 9 Stamina per square, and deals an extra
          1d6 damage.
        name: Metal
        cost: +2 EV
      - effect: The ram automatically resets at the start of each round.
        name: Repeating
        cost: +1 EV
      - effect: The ram automatically resets at the start of each turn.
        name: Rapid Repeating
        cost: +3 EV
      - effect: Multiple rams can be used to represent a larger mechanism, such as a
          stack of tumbling logs.
        name: Multiple Rams
        cost: +3 EV per additional ram
  - name: Hidden
    icon: ⭐️
    effects:
      - effect: The ram is hidden until triggered or detected.
~~~