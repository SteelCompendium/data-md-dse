---
file_basename: Shadow Elf Malice
file_dpath: Monsters/Elves Shadow/Features
item_id: shadow-elf-malice-malice-features
item_index: '27'
item_name: Shadow Elf Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:shadow-elf-malice-malice-features
scdc:
- 1.1.1:2.2:27
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Shadow Elf Malice
flavor: At the start of any shadow elf's turn, you can spend Malice to activate
  one of the following features.
features:
  - type: feature
    feature_type: trait
    name: Watch Me Disappear
    icon: ⭐️
    cost: 3 Malice
    effects:
      - effect: Each shadow elf acting this turn can attempt to hide as a free maneuver
          if they have concealment.
  - type: feature
    feature_type: trait
    name: Extra Dimension
    icon: ⭐️
    cost: 5 Malice
    effects:
      - effect: When any shadow elf acting this turn makes a strike against a target who
          has I < 2 in addition to the strike's regular effects, the target is
          bleeding (save ends) or slowed (save ends).
  - type: feature
    feature_type: trait
    name: Home Is Where the Hurt Is
    icon: 🌀
    cost: 10 Malice
    effects:
      - effect: The shadow elves synthesize a concentrated pocket manifold reminiscent
          of Equinox and graft it onto the encounter map. Until the end of the
          encounter, all creatures can see shadow elves in full color, and
          shadow elves no longer benefit from their Of the Umbra trait.
          Additionally, the potency of all shadow elf abilities increases by 2,
          and any enemy making a saving throw against an effect imposed by a
          shadow elf ability must roll an 8 or higher as they feel the effect
          across two worlds.
~~~