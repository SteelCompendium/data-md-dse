---
file_basename: Devil Malice
file_dpath: Monsters/Devils/Features
item_id: devil-malice-malice-features
item_index: '41'
item_name: Devil Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:devil-malice-malice-features
scdc:
- 1.1.1:2.2:41
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Devil Malice
flavor: At the start of any devil's turn, you can spend Malice to activate one
  of the following features.
features:
  - type: feature
    feature_type: trait
    name: Bureaucratic Tape
    icon: 👤
    cost: 3 Malice
    effects:
      - effect: One devil acting this turn uses a signature ability against an adjacent
          creature. On a tier 3 outcome, the target of the ability has a double
          bane on strikes (save ends).
  - type: feature
    feature_type: trait
    name: Underhanded Tactics
    icon: ⭐️
    cost: 5+ Malice
    effects:
      - effect: One or two devils can teleport to a space adjacent to one or more
          creatures who aren't hidden and make a free strike. For each 2
          additional Malice spent on this feature, one additional devil can
          teleport.
  - type: feature
    feature_type: trait
    name: Read the Small Print
    icon: 🌀
    cost: 7 Malice
    effects:
      - effect: Each enemy in the encounter is subject to a bad deal proposed by the
          devils. An enemy must choose between having damage weakness 5 or
          taking a bane on power rolls. The bad deal lasts until the end of the
          encounter.
~~~