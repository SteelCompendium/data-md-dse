---
file_basename: Meteor Dragon Malice
file_dpath: Monsters/Dragons/Features
item_id: meteor-dragon-malice-malice-features
item_index: '45'
item_name: Meteor Dragon Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:meteor-dragon-malice-malice-features
scdc:
- 1.1.1:2.2:45
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Meteor Dragon Malice
type: Malice Features
flavor: At the start of a meteor dragon's turn, you can spend Malice to activate
  one of the following features.
stats: []
features:
  - name: Liftoff
    icon: ⭐️
    cost: 3 Malice
    effects:
      - effect: The next time the dragon uses their Crescent Claws ability, they can
          also slide the target up to 5 squares. If the target is dragonsealed,
          the dragon can vertical slide them instead.
  - name: Solo Action
    icon: ☠️
    cost: 5 Malice
    effects:
      - effect: The dragon takes an additional main action on their turn. They can use
          this feature even if they are dazed.
  - name: Starfall
    icon: 🔳
    cost: 5 Malice
    effects:
      - effect: The dragon drops stars into five 2 cubes anywhere on the encounter map.
          The area is difficult terrain, and each creature and object in the
          area when it appears makes an **Agility test**.
        t1: 20 holy damage; slowed (save ends), prone
        t2: 16 holy damage; slowed (save ends)
        t3: 10 holy damage
  - name: Event Horizon
    icon: ☠️
    cost: 10 Malice
    effects:
      - effect: A black hole manifests as a 1 cube within 20 squares of the dragon in an
          unoccupied space. Each creature who has M < 5 and each object of size
          3 or smaller is vertical pulled 2 squares toward the area at the start
          of each round, ignoring stability. Any creature who starts their turn
          in the area or any object in the area at the end of the round suffers
          the effect of the dragon's Voidlight Breath ability, and the black
          hole disappears.
~~~