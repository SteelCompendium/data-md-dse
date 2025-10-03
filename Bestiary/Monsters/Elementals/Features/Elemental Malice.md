---
file_basename: Elemental Malice
file_dpath: Monsters/Elementals/Features
item_id: elemental-malice-malice-features
item_index: '44'
item_name: Elemental Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:elemental-malice-malice-features
scdc:
- 1.1.1:2.2:44
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Elemental Malice
flavor: At the start of any elemental's turn, you can spend Malice to activate
  one of the following features.
features:
  - type: feature
    feature_type: trait
    name: Elemental Swap
    icon: ⭐️
    cost: 3 Malice
    effects:
      - effect: Two elementals on the encounter map teleport to swap places, and each
          has damage immunity 2 until the end of the round.
  - type: feature
    feature_type: trait
    name: Split
    icon: 👤
    cost: 5 Malice
    effects:
      - effect: An elemental acting this turn cleaves themself into two separate
          elementals. Each elemental has the same statistics as the original,
          except that each has half the original's current Stamina and is one
          size smaller. Both elementals can then shift up to their speed.
  - type: feature
    feature_type: ability
    name: Convocation of Chaos
    icon: 🏹
    cost: 7 Malice
    keywords:
      - Magic
      - Ranged
    usage: Maneuver
    distance: Ranged 8
    target: Self or one elemental
    effects:
      - name: Effect
        effect: Until the end of the encounter, the target has a +5 bonus to speed and a
          +5 damage bonus to strikes. Additionally, whenever an elemental within
          the target's line of effect uses an ability with "Convocation" in the
          name, the target also gains the effects of that ability.
~~~