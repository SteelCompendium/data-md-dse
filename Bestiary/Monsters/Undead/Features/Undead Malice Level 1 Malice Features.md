---
file_basename: Undead Malice Level 1 Malice Features
file_dpath: Monsters/Undead/Features
include_parens_in_filename: 'true'
item_id: undead-malice-level-1-malice-features
item_index: '07'
item_name: Undead Malice (Level 1+ Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:undead-malice-level-1-malice-features
scdc:
- 1.1.1:2.2:07
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Undead Malice
type: + Malice Features
level: 1
flavor: At the start of any undead's turn, you can spend Malice to activate one
  of the following features.
stats: []
features:
  - name: Ravenous Horde
    icon: 🌀
    cost: 2 Malice
    effects:
      - effect: At the end of this round, each hero not already adjacent to one or more
          undead is beset by two **rotting zombies** who burst up from the
          ground to appear in adjacent unoccupied spaces. Each zombie is winded.
          This feature can't be used two rounds in a row.
  - name: Paranormal Fling
    icon: 🌀
    cost: 3 Malice
    effects:
      - effect: Up to three unattended objects on the encounter map rise to float 1
          square off the ground. Each object is then pulled 5 squares toward the
          nearest enemy within 3 squares of the object.
  - name: The Grasping, the Hungry
    icon: 🔳
    cost: 5 Malice
    effects:
      - effect: Ravenous and rotting undead arms burst forth from 9 connected squares of
          a vertical or horizontal surface. Any creature who ends their turn
          adjacent to an affected square makes an Agility test.
        t1: 5 damage; restrained (save ends)
        t2: 5 damage; restrained (EoT)
        t3: 5 damage
      - effect: While restrained this way, a creature takes 1d6 damage at the start of
          each of their turns.
        name: Effect
  - name: Dread March
    icon: ⭐️
    cost: 7+ Malice
    effects:
      - effect: Up to four undead in the encounter move up to their speed and can make a
          free strike. The number of undead affected increases by 1 for each
          additional Malice spent on this feature. If an undead is reduced to 0
          Stamina during this dread march, they don't die until the march is
          resolved.
~~~