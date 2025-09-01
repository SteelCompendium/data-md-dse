---
file_basename: Wyvern Malice Malice Features
file_dpath: Monsters/Wyverns/Features
item_id: wyvern-malice-malice-features
item_index: '15'
item_name: Wyvern Malice Malice Features
scc:
- mcdm.monsters.v1:monster.feature:wyvern-malice-malice-features
scdc:
- 1.1.1:2.2:15
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Wyvern Malice Malice Features
flavor: At the start of any wyvern's turn, you can spend Malice to activate one
  of the following features.
stats: []
features:
  - name: Simmering Anger
    icon: 🗡
    cost: 3 Malice
    effects:
      - effect: One wyvern in the encounter can make a free strike against each enemy
          adjacent to them.
  - name: Boiling Fury
    icon: ⭐️
    cost: 5 Malice
    effects:
      - effect: Until the end of the round, each wyvern in the encounter has a double
          edge on strikes and can use their signature ability instead of a free
          strike when making opportunity attacks.
  - name: Overflowing Rage
    icon: 🌀
    cost: 7 Malice
    effects:
      - effect: Every wyvern's anger fills the encounter map with a thick miasma of
          hatred. Each enemy in the encounter makes an **Intuition test**.
        t1: The target is taunted by the nearest creature or object (save ends). While
          the target is taunted this way, power rolls against them have a double
          edge.
        t2: The target is taunted by the nearest creature or object (save ends).
        t3: No effect.
~~~