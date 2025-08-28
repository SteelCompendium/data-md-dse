---
file_basename: Crucible Dragon Malice
file_dpath: Monsters/Dragons/Features
item_id: crucible-dragon-malice-malice-features
item_index: '48'
item_name: Crucible Dragon Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:crucible-dragon-malice-malice-features
scdc:
- 1.1.1:2.2:48
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Crucible Dragon Malice
type: Malice Features
flavor: At the start of a crucible dragon's turn, you can spend Malice to
  activate one of the following features.
stats: []
features:
  - name: Swordfall
    icon: 🔳
    cost: 3 Malice
    effects:
      - effect: While the dragon is flying, they shape themself into a blade and fall.
          Each creature and object in the dragon's space when they hit the
          ground and in a 6 x 4 line within 1 square of the dragon takes 7
          damage. A creature who takes this damage and has A < 4 takes 4 extra
          damage per square the dragon fell and is restrained (save ends). A
          creature not restrained this way can move into the nearest unoccupied
          space.
  - name: Shower of Blades
    icon: 🔳
    cost: 5 Malice
    effects:
      - effect: The dragon shakes loose a cloud of shattered weapons in a 6 x 4 line
          within 1 square of them. Each creature and object in the area makes an
          **Agility test**.
        t1: 16 damage; bleeding (save ends)
        t2: 13 damage; bleeding (EoT)
        t3: 7 damage
  - name: Solo Action
    icon: ☠️
    cost: 5 Malice
    effects:
      - effect: The dragon takes an additional main action on their turn. They can use
          this feature even if they are dazed.
  - name: Meltdown
    icon: 🌀
    cost: 7 Malice
    effects:
      - effect: The dragon superheats the ground across the encounter map until the end
          of the round. Any enemy who starts their turn on the ground is slagged
          as if affected by the dragon's Slag Spew ability.
~~~