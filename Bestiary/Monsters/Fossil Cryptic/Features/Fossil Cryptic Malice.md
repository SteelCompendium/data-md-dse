---
file_basename: Fossil Cryptic Malice
file_dpath: Monsters/Fossil Cryptic/Features
item_id: fossil-cryptic-malice-malice-features
item_index: '64'
item_name: Fossil Cryptic Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:fossil-cryptic-malice-malice-features
scdc:
- 1.1.1:2.2:64
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Fossil Cryptic Malice
flavor: At the start of a fossil cryptic's turn, you can spend Malice to
  activate one of the following features.
features:
  - type: feature
    feature_type: trait
    name: Floor Mosaic
    icon: 🏹
    cost: 3 Malice
    effects:
      - effect: The fossil cryptic slides one creature on the ground up to 5 squares. If
          the creature is prone, this forced movement ignores stability.
  - type: feature
    feature_type: trait
    name: Solo Action
    icon: ☠️
    cost: 5 Malice
    effects:
      - effect: The fossil cryptic takes an additional main action on their turn. They
          can use this feature even if they are dazed.
  - type: feature
    feature_type: trait
    name: Stone Pillars
    icon: 🔳
    cost: 5 Malice
    effects:
      - effect: Two pillars of stone 1 square wide either thrust up out of the ground or
          jut down from the ceiling anywhere on the encounter map, to a height
          of up to 5 squares. A creature in the area of a pillar before it
          appears is knocked prone on its surface. If the creature comes into
          contact with the ceiling above or the floor beneath the pillar and has
          M < 2 they are restrained (save ends).
  - type: feature
    feature_type: trait
    name: Choking Dust
    icon: 🌀
    cost: 10 Malice
    effects:
      - effect: The air across the encounter map is thick with dust until the end of the
          encounter. Each enemy in the dust is suffocating. Additionally, at the
          end of each round, each enemy in the dust makes a **Might test**.
        tier1: Until the end of the enemy's next turn, their stability is reduced to 0,
          and any forced movement effects targeting them gain a +2 bonus to the
          distance moved.
        tier2: The enemy's stability is halved (EoT).
        tier3: No effect.
~~~