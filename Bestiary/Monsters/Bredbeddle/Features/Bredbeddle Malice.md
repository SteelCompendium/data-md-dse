---
file_basename: Bredbeddle Malice
file_dpath: Monsters/Bredbeddle/Features
item_id: bredbeddle-malice-malice-features
item_index: '25'
item_name: Bredbeddle Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:bredbeddle-malice-malice-features
scdc:
- 1.1.1:2.2:25
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Bredbeddle Malice
flavor: At the start of a bredbeddle's turn, you can spend Malice to activate
  one of the following features.
features:
  - type: feature
    feature_type: trait
    name: Engreen
    icon: ⭐️
    cost: 3 Malice
    effects:
      - effect: The bredbeddle's axe lengthens and turns a ghastly green, granting a +1
          bonus to the distance of the bredbeddle's melee strikes and the
          dimensions of their burst area abilities until the end of their turn.
  - type: feature
    feature_type: trait
    name: Shadow Stockade
    icon: 🔳
    cost: 5 Malice
    effects:
      - effect: A ghostly size 1L stockade seeps out from under the bredbeddle's feet to
          fill an unoccupied square within 10 squares. When a size 1L or smaller
          enemy enters the stockade's square, they are restrained (save ends).
          When a restrained creature is no longer restrained, the stockade fades
          away. At the start of each of the bredbeddle's turns, they can slide
          an active stockade and any creature in it up to 5 squares.
  - type: feature
    feature_type: trait
    name: Solo Action
    icon: ☠️
    cost: 5 Malice
    effects:
      - effect: The bredbeddle takes an additional main action on their turn. They can
          use this feature even if they are dazed.
  - type: feature
    feature_type: trait
    name: Green Phantom
    icon: 🌀
    cost: 7 Malice
    effects:
      - effect: A phantom second bredbeddle phases into view, appearing in an unoccupied
          space anywhere on the encounter map, then vanishing at the end of the
          round. The phantom bredbeddle shares the original bredbeddle's
          statistics but has 24 Stamina, corruption immunity 10, and can fly.
          The phantom bredbeddle can take one turn and use any of the
          bredbeddle's abilities except for villain actions. Only one phantom
          bredbeddle can be active at a time.
~~~