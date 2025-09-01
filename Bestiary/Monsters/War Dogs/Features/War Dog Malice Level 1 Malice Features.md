---
file_basename: War Dog Malice Level 1 Malice Features
file_dpath: Monsters/War Dogs/Features
include_parens_in_filename: 'true'
item_id: war-dog-malice-level-1-malice-features
item_index: '60'
item_name: War Dog Malice (Level 1+ Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:war-dog-malice-level-1-malice-features
scdc:
- 1.1.1:2.2:60
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: War Dog Malice
type: + Malice Features
level: 1
flavor: At the start of any war dog's turn, you can spend Malice to activate one
  of the following features.
features:
  - name: Reconstitute
    icon: 👤
    cost: 3 Malice
    effects:
      - effect: One war dog acting this turn tears apart a nearby corpse of a humanoid
          and incorporates its body parts into their own. The war dog regains
          Stamina equal to 5 times their level.
  - name: Fire for Effect
    icon: 🔳
    cost: 5 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    type: Maneuver
    distance: 4 cube within 10
    target: Each creature in the area
    effects:
      - name: Effect
        effect: Each target makes an **Agility test**. The same condition is imposed on
          each affected target.
        t1: 5 fire damage; slowed or weakened (save ends)
        t2: 5 fire damage; slowed or weakened (EoT)
        t3: 5 fire damage
  - name: Fodder Run
    icon: ⭐️
    cost: 7 Malice
    effects:
      - effect: Each war dog minion in the encounter shifts up to their speed and can
          make a free strike. A minion who does so is then reduced to 0 Stamina.
~~~