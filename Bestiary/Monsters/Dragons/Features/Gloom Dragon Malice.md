---
file_basename: Gloom Dragon Malice
file_dpath: Monsters/Dragons/Features
item_id: gloom-dragon-malice-malice-features
item_index: '52'
item_name: Gloom Dragon Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:gloom-dragon-malice-malice-features
scdc:
- 1.1.1:2.2:52
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Gloom Dragon Malice
flavor: At the start of a gloom dragon's turn, you can spend Malice to activate
  one of the following features.
features:
  - type: feature
    feature_type: trait
    name: Dread and Terror
    icon: ⭐️
    cost: 3 Malice
    effects:
      - effect: The dragon thickens the fog of their Gloaming Wyrmscale Aura trait and
          the horrors within it. Each creature in the area takes a bane on
          strikes made against the dragon until the start of the dragon's next
          turn.
  - type: feature
    feature_type: trait
    name: Doleful Visions
    icon: 🔳
    cost: 5 Malice
    effects:
      - effect: The dragon manifests four 2 cubes of nightmarish apparitions anywhere on
          the encounter map. Each creature in the area when it appears makes an
          **Intuition test**.
        tier1: 14 damage; dazed (save ends)
        tier2: 11 damage; dazed (EoT)
        tier3: 6 damage
  - type: feature
    feature_type: trait
    name: Solo Action
    icon: ☠️
    cost: 5 Malice
    effects:
      - effect: The dragon takes an additional main action on their turn. They can use
          this feature even if they are dazed.
  - type: feature
    feature_type: trait
    name: Phantasmagoria!
    icon: 🔳
    cost: 7 Malice
    effects:
      - effect: The dragon summons macabre, disquieting phantasms in a 10 cube within 1
          square that lasts until the end of the encounter. Any enemy who enters
          the area for the first time in a round or starts their turn there
          takes 6 psychic damage, or 8 psychic damage if they are dragonsealed
          by the gloom dragon. Additionally, the enemy's Intuition score is
          treated as 1 lower for the purpose of resisting potencies until the
          end of the encounter.
~~~