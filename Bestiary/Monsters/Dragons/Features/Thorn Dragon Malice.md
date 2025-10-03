---
file_basename: Thorn Dragon Malice
file_dpath: Monsters/Dragons/Features
item_id: thorn-dragon-malice-malice-features
item_index: '49'
item_name: Thorn Dragon Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:thorn-dragon-malice-malice-features
scdc:
- 1.1.1:2.2:49
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Thorn Dragon Malice
flavor: At the start of a thorn dragon's turn, you can spend Malice to activate
  one of the following features.
features:
  - type: feature
    feature_type: trait
    name: Cage of Thorns
    icon: ⭐️
    cost: 3 Malice
    effects:
      - effect: A cage of thorns grows around one dragonsealed enemy on the encounter
          map, making that enemy restrained until the end of their next turn.
  - type: feature
    feature_type: trait
    name: Bramble Barricade
    icon: 🔳
    cost: 5 Malice
    effects:
      - effect: The dragon grows a 10 wall of briars in unoccupied spaces on the
          encounter map. The wall blocks line of effect for all creatures except
          the dragon. Each square of the wall has 5 Stamina and fire weakness 5.
          The area can be moved through but is difficult terrain. Any creature
          who is force moved into or within the area takes 1 damage for each
          square of the area entered and is bleeding until the end of their next
          turn.
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
    name: Afflictive Overgrowth
    icon: 🌀
    cost: 7 Malice
    effects:
      - effect: The dragon summons poisonous, biting thorns around their foes. Each
          enemy on the encounter map makes an **Agility test**.
        tier1: 12 poison damage; restrained (save ends)
        tier2: 9 poison damage; bleeding (save ends)
        tier3: 5 poison damage; bleeding (EoT)
~~~