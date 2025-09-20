---
file_basename: Rival Malice Level 1 Malice Features
file_dpath: Monsters/Rivals/Features
include_parens_in_filename: 'true'
item_id: rival-malice-level-1-malice-features
item_index: '03'
item_name: Rival Malice (Level 1+ Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:rival-malice-level-1-malice-features
scdc:
- 1.1.1:2.2:03
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: + Malice Features
name: Rival Malice
level: 1
flavor: At the start of any rival's turn, you can spend Malice to activate one
  of the following features.
features:
  - type: feature
    feature_type: trait
    name: Work as One
    icon: ⭐️
    cost: 3 Malice
    effects:
      - effect: Until the end of the round, each rival can impose a bane on a strike
          made against an adjacent rival as a free triggered action.
  - type: feature
    feature_type: trait
    name: We Just Do It Better
    icon: ⭐️
    cost: 3 Malice
    effects:
      - effect: Until the end of the round, whenever any rival makes a power roll
          against the target of their Rivalry trait, they roll a d3 and add it
          to the power roll.
  - type: feature
    feature_type: trait
    name: Check Out Our Loot
    icon: 🔳
    cost: 5 Malice
    effects:
      - effect: "One rival pulls out a magic consumable and hurls it, targeting a 5 x 1
          line within 1 square of them or a 3 cube within 10 squares of them.
          Each enemy in the area makes an Agility test. The rival chooses a
          damage type and a condition for the outcome of the test from one of
          the following pairs: sonic damage and dazed, poison damage and
          weakened, or fire damage and frightened."
        tier1: 11 damage; the condition affects the target (save ends)
        tier2: 8 damage; the condition affects the target (EoT)
        tier3: 5 damage
  - type: feature
    feature_type: trait
    name: Calling the Shots
    icon: ⭐️
    cost: 7 Malice
    effects:
      - effect: Each rival regains 10 Stamina. Until the end of the round, whenever a
          rival uses an ability against an enemy, each other rival adjacent to
          that enemy can make a free strike against them.
  - type: feature
    feature_type: trait
    name: Coordinated Takedown
    icon: ⭐️
    cost: 10 Malice
    effects:
      - effect: Each rival moves up to their speed and uses a main action or maneuver
          that doesn't cost Malice.
~~~