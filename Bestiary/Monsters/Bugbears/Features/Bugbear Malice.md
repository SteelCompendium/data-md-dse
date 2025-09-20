---
file_basename: Bugbear Malice
file_dpath: Monsters/Bugbears/Features
item_id: bugbear-malice-malice-features
item_index: '40'
item_name: Bugbear Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:bugbear-malice-malice-features
scdc:
- 1.1.1:2.2:40
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Bugbear Malice
flavor: At the start of any bugbear's turn, you can spend Malice to activate one
  of the following features.
features:
  - type: feature
    feature_type: trait
    name: Goblin Malice Features
    icon: ⭐️
    cost: 3-7 Malice
    effects:
      - effect: The bugbear activates a Malice Feature available to goblins.
  - type: feature
    feature_type: trait
    name: Grab Iron Ball
    icon: 👤
    cost: 3+ Malice
    effects:
      - effect: For every 3 Malice spent, one non-minion bugbear acting this turn grabs
          an iron ball and can use a maneuver to throw it at a creature within 5
          squares of them. The creature takes damage equal to 8 - the number of
          squares the iron ball was thrown, and if they have M < 1, they are
          slowed (save ends).
  - type: feature
    feature_type: trait
    name: Grab Javelin
    icon: 👤
    cost: 5+ Malice
    effects:
      - effect: For every 5 Malice spent, one non-minion bugbear acting this turn grabs
          a javelin and can use a maneuver to throw it at a creature within 5
          squares of them. The creature takes damage equal to 12 - the number of
          squares the javelin was thrown, and if they have M < 1, they are
          bleeding (save ends). While a creature is bleeding this way, any ally
          of the bugbear within 2 squares of them can use a free maneuver to
          pull the bleeding creature up to 2 squares.
  - type: feature
    feature_type: trait
    name: Show Them the Great Fear
    icon: 🌀
    cost: 10 Malice
    effects:
      - effect: A bugbear infuses the encounter map with bu'gathic magic. Until the end
          of the encounter, all bugbears and allies have their speed doubled and
          can automatically climb at full speed while moving. Additionally, if
          the target of any bugbear or ally's strike has I < 1, the target is
          also frightened (save ends) and must move their speed in a straight
          line away from the creature who made the strike.
~~~