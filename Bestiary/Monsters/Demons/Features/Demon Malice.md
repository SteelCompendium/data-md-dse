---
file_basename: Demon Malice
file_dpath: Monsters/Demons/Features
item_id: demon-malice-level-10-malice-features
item_index: '32'
item_name: Demon Malice (Level 10+ Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:demon-malice-level-10-malice-features
scdc:
- 1.1.1:2.2:32
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Demon Malice
type: + Malice Features
level: 10
flavor: At the start of any level 10 or higher demon's turn, you can spend
  Malice to activate one of the following features.
stats: []
features:
  - name: Prior Malice Features
    icon: ⭐️
    cost: 3-7 Malice
    effects:
      - effect: The demon activates a Malice feature available to demons of level 9 or
          lower.
  - name: Soul Flense
    icon: ❇️
    cost: 7 Malice
    effects:
      - effect: One demon acting this turn unleashes their pent-up agony and pain on
          every non-demon in a 5 burst. Each target makes a **Presence test**.
        t1: 10 corruption damage; the target is soul flensed
        t2: The target is soul flensed
        t3: No effect.
      - effect: The demon removes all conditions and effects on themself that can be
          ended by a saving throw, and transfers all those effects to each
          creature soul flensed this way.
        name: Effect
~~~