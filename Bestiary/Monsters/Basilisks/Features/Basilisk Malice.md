---
file_basename: Basilisk Malice
file_dpath: Monsters/Basilisks/Features
item_id: basilisk-malice-malice-features
item_index: '46'
item_name: Basilisk Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:basilisk-malice-malice-features
scdc:
- 1.1.1:2.2:46
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Basilisk Malice
flavor: At the start of any basilisk's turn, you can spend Malice to activate
  one of the following features.
features:
  - type: feature
    feature_type: trait
    name: Stone Swim
    icon: ⭐️
    cost: 3+ Malice
    effects:
      - effect: A basilisk acting this turn can burrow until the start of their next
          turn, and moves up to their speed. They have damage immunity 2 while
          underground. The basilisk can burrow through stone, but can't drag
          other creatures underground when they do so. At the start of each of
          the basilisk's turns, the Director can spend 1 Malice to let the
          basilisk continue burrowing.
  - type: feature
    feature_type: ability
    name: Upchuck
    icon: 🔳
    cost: 5 Malice
    keywords:
      - Area
      - Weapon
    usage: Main action
    distance: 3 cube within 10
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: The basilisk spits up a chunk of partly digested stone.
      - roll: Power Roll + 2
        tier1: 4 damage
        tier2: 4 damage; A < 1 2 damage, prone
        tier3: 4 damage; A < 2 5 damage, prone and can't stand (save ends)
  - type: feature
    feature_type: trait
    name: Walleye
    icon: 🔳
    cost: 7 Malice
    effects:
      - effect: A basilisk spews reflective spittle across an adjacent vertical surface
          in a 3-square-by-3-square area. The basilisk can use their Petrifying
          Eye Beams ability to target a square in the area, causing the area and
          distance of that ability to become a 20 x 3 line within 1 square of
          the wall.
~~~