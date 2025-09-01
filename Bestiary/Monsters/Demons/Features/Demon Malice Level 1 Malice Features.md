---
file_basename: Demon Malice Level 1 Malice Features
file_dpath: Monsters/Demons/Features
include_parens_in_filename: 'true'
item_id: demon-malice-level-1-malice-features
item_index: '36'
item_name: Demon Malice (Level 1+ Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:demon-malice-level-1-malice-features
scdc:
- 1.1.1:2.2:36
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Demon Malice
type: + Malice Features
level: 1
flavor: At the start of any demon's turn, you can spend Malice to activate one
  of the following features.
features:
  - name: Soulburn
    icon: ⭐️
    cost: 3 Malice
    effects:
      - effect: Each demon acting this turn has a double edge on abilities.
  - name: Abyssal Evolution
    icon: 🌀
    cost: 7 Malice
    effects:
      - effect: A demon minion of your choice transforms into a non-minion horde demon
          of the same level.
  - name: Abyssal Rift
    icon: 🔳
    cost: 7 Malice
    effects:
      - effect: Two size 2 rifts to the Abyssal Wasteland appear at locations of your
          choice. Any demon can use an abyssal rift as a portal to another
          abyssal rift in the encounter, moving into any space in one rift and
          appearing immediately in any unoccupied space in the other rift. A
          non-demon who enters a rift for the first time in a round or starts
          their turn there takes corruption damage equal to the level of the
          highest-level demon on the encounter map. An abyssal rift is an
          immovable object that has 25 Stamina, damage immunity 2, and holy
          weakness 5. The rift closes when there are no demons remaining on the
          encounter map. Additionally, a creature who has the Magic or Psionics
          skill can make a Reason test or Intuition test as a maneuver while
          adjacent to a rift to destabilize and close it.
        t1: The rift remains open and regains 5 Stamina.
        t2: The rift remains open.
        t3: The rift closes.
~~~