---
file_basename: Column of Blades
file_dpath: Dynamic Terrain/Mechanisms
item_id: column-of-blades-level-3-fortification-defender
item_index: '04'
item_name: Column of Blades (Level 3 Fortification Defender)
scc:
- mcdm.monsters.v1:dynamic-terrain.mechanism:column-of-blades-level-3-fortification-defender
scdc:
- 1.1.1:4.1:04
source: mcdm.monsters.v1
type: dynamic-terrain/mechanism
---

~~~ds-featureblock
name: Column of Blades
type: Fortification Defender
level: 3
ev: "3"
flavor: A spinning wooden column is affixed with sharp blades to slash the unwary.
stamina: "5"
size: 1L
features:
  - name: Deactivate
    icon: 🌀
    effects:
      - effect: The column of blades must be completely destroyed.
  - name: Activate
    icon: ❕
    effects:
      - effect: A creature or object moves adjacent to the column of blades.
      - effect: The **Spinning Blades** ability.
        name: Effect
  - name: Spinning Blades
    icon: ❗️
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Free triggered action
    distance: Melee 1
    target: The triggering creature or object
    trigger: A creature or object moves within distance of the column.
    effects:
      - roll: Power Roll + 2
        t1: 4 damage
        t2: 6 damage; M < 2 bleeding (save ends)
        t3: 9 damage; M < 3 bleeding (save ends)
  - name: Upgrades
    icon: ⭐️
    effects:
      - effect: "**Stone Column (+1 EV)** The column is made of stone and has 8
          Stamina."
      - effect: "**Metal Column (+1 EV)** The column is made of metal and has 11
          Stamina."
      - effect: "**Concealed (+1 EV)** The blades are concealed inside the column, which
          remains motionless until triggered."
      - effect: "**Spiked Flails (+4 EV)** Instead of blades, the column is affixed with
          heavy spiked balls attached by long chains. The **Whirling Flails**
          ability replaces **Spinning Blades**."
  - name: Whirling Flails
    icon: ❗️
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Free triggered action
    distance: Melee 2
    target: The triggering creature or object
    trigger: |-
      A creature or object moves within distance of the column.
      - **≤11:** 5 damage
      - **12-16:** 8 damage; M < 2 dazed (save ends)
      - **17+:** 11 damage; M < 3 dazed (save ends)
    effects: []
  - name: Allied Awareness
    icon: ⭐️
    effects:
      - effect: Allies who shift don't trigger the column. A creature observing an ally
          shift this way can make an **Intuition test** to shift in imitation of
          their movements.
      - roll: Power Roll + 2
        t1: The creature triggers the column and the column's ability gains an edge.
        t2: The creature triggers the column.
        t3: The creature doesn't trigger the column.
~~~