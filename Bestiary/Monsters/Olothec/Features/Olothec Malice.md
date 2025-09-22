---
file_basename: Olothec Malice
file_dpath: Monsters/Olothec/Features
item_id: olothec-malice-malice-features
item_index: '13'
item_name: Olothec Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:olothec-malice-malice-features
scdc:
- 1.1.1:2.2:13
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Olothec Malice
flavor: At the start of an olothec's turn, you can spend Malice to activate one
  of the following features.
features:
  - type: feature
    feature_type: trait
    name: Solo Action
    icon: ☠️
    cost: 4 Malice
    effects:
      - effect: The olothec takes an additional main action on their turn. They can use
          this feature even if they are dazed.
  - type: feature
    feature_type: ability
    name: Writhing Envelopment
    icon: 🗡
    cost: 4 Malice
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 3
    target: One slimed, transformed, or devolved creature
    effects:
      - roll: Power Roll + 4
        tier1: 11 psychic damage; A < 2 grabbed
        tier2: 17 psychic damage; A < 3 grabbed
        tier3: 20 psychic damage; A < 4 grabbed
      - name: Effect
        effect: The olothec can pull a target grabbed this way adjacent to them. While
          grabbed this way, a target can't make saving throws to end any other
          effects, and the olothec has a double edge on strikes against them.
  - type: feature
    feature_type: trait
    name: Memory of Chaos
    icon: ❇️
    cost: 6 Malice
    effects:
      - effect: The olothec broadcasts their memory of the universe in its primordial
          state—a sweeping cacophony of transcendental irrationality and
          unceasing change. Until the end of the encounter, any creature who
          starts their turn within 3 squares of the olothec and has R < 3 is
          dazed and slowed until the end of their next turn).
~~~