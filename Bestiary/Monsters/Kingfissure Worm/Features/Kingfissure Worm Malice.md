---
file_basename: Kingfissure Worm Malice
file_dpath: Monsters/Kingfissure Worm/Features
item_id: kingfissure-worm-malice-malice-features
item_index: '34'
item_name: Kingfissure Worm Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:kingfissure-worm-malice-malice-features
scdc:
- 1.1.1:2.2:34
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Kingfissure Worm Malice
type: Malice Features
flavor: At the start of a kingfissure worm's turn or when an action's trigger
  occurs, you can spend Malice to activate one of the following features.
features:
  - name: Aftershock
    icon: ❗️
    cost: 3 Malice
    keywords:
      - "-"
    type: Free triggered action
    distance: Self
    target: Self
    trigger: A creature deals damage to the kingfissure worm or one of their tongues.
    effects:
      - effect: Each creature within 5 squares of the kingfissure worm takes 5 damage,
          and if they have A < 4 they are knocked prone. The kingfissure worm
          can use this ability only once per round.
        name: Effect
  - name: Solo Action
    icon: ☠️
    cost: 5 Malice
    effects:
      - effect: The kingfissure worm takes an additional main action on their turn. They
          can use this feature even if they are dazed.
  - name: Spontaneous Regeneration
    icon: 👤
    cost: 5 Malice
    effects:
      - effect: The kingfissure worm loses 35 Stamina and regrows one tongue, to a
          maximum of three tongues. The worm is then dazed until the end of
          their turn.
  - name: Megaquake
    icon: ❇️
    cost: 7 Malice
    keywords:
      - Area
      - Weapon
    type: Main action
    distance: 5 burst
    target: Each enemy and object in the area
    effects:
      - roll: Power Roll + 5
        t1: 8 damage; M < 3 slide 5
        t2: 13 damage; M < 4 slide 5
        t3: 17 damage; M < 5 slide 5
      - effect: Until the end of the next round, each target takes a −3 penalty to
          stability, treats all terrain as difficult terrain, and takes 10
          damage whenever they are knocked prone.
        name: Effect
~~~