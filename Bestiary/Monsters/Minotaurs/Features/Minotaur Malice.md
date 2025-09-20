---
file_basename: Minotaur Malice
file_dpath: Monsters/Minotaurs/Features
item_id: minotaur-malice-malice-features
item_index: '22'
item_name: Minotaur Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:minotaur-malice-malice-features
scdc:
- 1.1.1:2.2:22
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Minotaur Malice
flavor: At the start of any minotaur's turn, you can spend Malice to activate
  one of the following features.
features:
  - type: feature
    feature_type: trait
    name: Bull Rush
    icon: 👤
    cost: 3 Malice
    effects:
      - effect: For each 3 Malice spent, one minotaur acting this turn gains a +4 bonus
          to speed and ignores difficult terrain until the start of their next
          turn.
  - type: feature
    feature_type: trait
    name: Cut the... Nonsense!
    icon: 👤
    cost: 5 Malice
    effects:
      - effect: One minotaur acting this turn halves any damage they take, and can use
          the Knockback maneuver as a free triggered action whenever an enemy
          comes adjacent to them, all until the start of their next turn.
  - type: feature
    feature_type: trait
    name: Bullseye
    icon: ❇️
    cost: 7 Malice
    effects:
      - effect: All minotaurs in the encounter fill the area around them with psychic
          impressions of feeling lost and isolated. Each enemy within 5 squares
          of a minotaur is teleported up to 5 squares and makes an **Intuition
          test**.
        tier1: The target has line of effect only within 3 squares and is frightened of
          all minotaurs (save ends).
        tier2: The target has line of effect only within 3 squares (EoT).
        tier3: No effect.
~~~