---
file_basename: War Dog Malice Level 10 Malice Features
file_dpath: Monsters/War Dogs/Features
include_parens_in_filename: 'true'
item_id: war-dog-malice-level-10-malice-features
item_index: '59'
item_name: War Dog Malice (Level 10+ Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:war-dog-malice-level-10-malice-features
scdc:
- 1.1.1:2.2:59
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: War Dog Malice
type: + Malice Features
level: 10
flavor: At the start of any level 10 or higher war dog's turn, you can spend
  Malice to activate one of the following features.
features:
  - name: Prior Malice Features
    icon: ⭐️
    cost: 3-7 Malice
    effects:
      - effect: The war dog activates a Malice feature available to war dogs of level 9
          or lower.
  - name: Cry Havoc
    icon: ❇️
    cost: 7 Malice
    keywords:
      - Area
      - Magic
    type: Maneuver
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 5
        t1: 7 psychic damage
        t2: 11 psychic damage; P < 4 frightened (save ends)
        t3: 14 psychic damage; P < 5 frightened (save ends)
      - effect: Each war dog within distance deals an extra 15 damage with strikes until
          the end of their next turn. Additionally, they end any effect on them
          that can be ended by a saving throw or that ends at the end of their
          turn, then shift up to their speed and can make a free strike.
        name: Effect
      - effect: This ability can't be used by a minion.
        name: Special
~~~