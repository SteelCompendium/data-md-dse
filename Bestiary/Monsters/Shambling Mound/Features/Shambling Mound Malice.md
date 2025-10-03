---
file_basename: Shambling Mound Malice
file_dpath: Monsters/Shambling Mound/Features
item_id: shambling-mound-malice-malice-features
item_index: '56'
item_name: Shambling Mound Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:shambling-mound-malice-malice-features
scdc:
- 1.1.1:2.2:56
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Shambling Mound Malice
flavor: At the start of a shambling mound's turn, you can spend Malice to
  activate one of the following features.
features:
  - type: feature
    feature_type: trait
    name: Poisoned Vines
    icon: 👤
    cost: 3 Malice
    effects:
      - effect: The shambling mound seeps noxious residue from their vines. The next
          time they use their Vine Lash ability before the end of their next
          turn, they deal an extra 12 poison damage to each target.
  - type: feature
    feature_type: trait
    name: Frenzy Lash
    icon: ❇️
    cost: 5 Malice
    effects:
      - effect: The shambling mound lashes out at each enemy within 10 squares of them,
          driving them back or into the air. Each target makes an **Agility
          test**.
        tier1: 7 damage; push 7 or vertical push 3; restrained (save ends)
        tier2: 6 damage; push 5 or vertical push 2
        tier3: 3 damage
  - type: feature
    feature_type: trait
    name: Solo Action
    icon: ☠️
    cost: 5 Malice
    effects:
      - effect: The shambling mound takes an additional main action on their turn. They
          can use this feature even if they are dazed.
  - type: feature
    feature_type: trait
    name: Leeching Wilds
    icon: ❇️
    cost: 7 Malice
    effects:
      - effect: Until the end of the shambling mound's next turn, the area within 10
          squares of them is difficult terrain for enemies, and any enemy in the
          area takes a bane on power rolls. Any enemy who starts their turn in
          the area takes 4 acid damage, and the shambling mound regains an equal
          amount of Stamina.
~~~