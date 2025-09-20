---
file_basename: Ogre Malice
file_dpath: Monsters/Ogres/Features
item_id: ogre-malice-malice-features
item_index: '02'
item_name: Ogre Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:ogre-malice-malice-features
scdc:
- 1.1.1:2.2:02
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Ogre Malice
flavor: At the start of any ogre's turn, you can spend Malice to activate one of
  the following features.
features:
  - type: feature
    feature_type: trait
    name: Shockwave
    icon: ❇️
    cost: 3 Malice
    effects:
      - effect: One ogre acting this turn jumps and lands on their rear, causing a 3
          burst shockwave. Each size 1 creature in the area makes a **Might
          test** or **Agility test**.
        tier1: 5 damage; vertical push 3
        tier2: 4 damage; vertical push 2
        tier3: Push 1
  - type: feature
    feature_type: trait
    name: Bully
    icon: 🌀
    cost: 5 Malice
    effects:
      - effect: Each ogre in the encounter shifts up to their speed and can make a free
          strike. If they can, they gang up on the same target rather than
          picking different targets.
  - type: feature
    feature_type: trait
    name: Rampage
    icon: ⭐️
    cost: 7 Malice
    effects:
      - effect: Until the end of the round, each ogre has damage immunity 5 and deals an
          extra 5 damage with abilities, and heroic abilities that target any
          ogre have their Heroic Resource cost reduced by 1 (to a minimum of 1).
~~~