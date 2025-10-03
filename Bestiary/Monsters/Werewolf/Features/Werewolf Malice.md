---
file_basename: Werewolf Malice
file_dpath: Monsters/Werewolf/Features
item_id: werewolf-malice-malice-features
item_index: '47'
item_name: Werewolf Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:werewolf-malice-malice-features
scdc:
- 1.1.1:2.2:47
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Werewolf Malice
flavor: At the start of a werewolf's turn, you can spend Malice to activate one
  of the following features.
features:
  - type: feature
    feature_type: trait
    name: Blood In Their Eyes
    icon: ⭐️
    cost: 3 Malice
    effects:
      - effect: The werewolf gains 10 temporary Stamina and a +3 bonus to speed until
          the end of their turn. The werewolf can't use this feature if they
          took any holy damage since ending their last turn.
  - type: feature
    feature_type: trait
    name: Solo Action
    icon: ☠️
    cost: 5 Malice
    effects:
      - effect: The werewolf takes an additional main action on their turn. They can use
          this feature even if they are dazed.
  - type: feature
    feature_type: trait
    name: Moonfall
    icon: 🌀
    cost: 10 Malice
    effects:
      - effect: Until the end of the encounter, the encounter map turns to night and the
          moon appears impossibly huge in the sky. The werewolf can take an
          additional move action or maneuver on each of their turns while they
          have line of effect to the moon. Any creature who ends their turn with
          line of effect to the moon with 1 or more rage gains 2 rag.
~~~