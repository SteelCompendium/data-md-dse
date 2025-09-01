---
file_basename: Lizardfolk Malice
file_dpath: Monsters/Lizardfolks/Features
item_id: lizardfolk-malice-malice-features
item_index: '05'
item_name: Lizardfolk Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:lizardfolk-malice-malice-features
scdc:
- 1.1.1:2.2:05
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Lizardfolk Malice
type: Malice Features
flavor: At the start of any lizardfolk's turn, you can spend Malice to activate
  one of the following features.
features:
  - name: Net Trap
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
      - Ranged
      - Weapon
    type: Maneuver
    distance: 1 cube within 3
    target: Special
    effects:
      - name: Effect
        effect: A lizardfolk acting this turn sets up a net trap into the area. The
          first time an enemy steps into a square with a net trap, they make an
          **Agility test**. If the creature was unaware of the trap, they take a
          bane on the test.
        t1: Restrained (save ends).
        t2: Restrained (Eot).
        t3: No effect.
      - effect: Any creature not also restrained by a net trap who is adjacent to a
          creature restrained by the trap can free them as a maneuver.
        name: Effect
  - name: Water Pit
    icon: 🔳
    cost: 5 Malice
    effects:
      - effect: A lizardfolk acting this turn unearths a magical size 2 pit that is 2
          squares deep and filled with water. Any lizardfolk who moves into,
          then exits the pit on their turn gains 10 temporary Stamina, regrows
          their tail if applicable, and ends one effect on them that can be
          ended by a saving throw. While adjacent to the pit, any creature who
          can burrow or who has the Nature skill can make a **Might test** or a
          **Reason test** to drain it.
        t1: The creature falls into the pit and is knocked prone.
        t2: The creature fails to empty the pit.
        t3: The pit empties of water.
  - name: Flood the Shores
    icon: 🌀
    cost: 7 Malice
    effects:
      - effect: Waist-high water floods the entire encounter map. Any lizardfolk
          submerged in water gains an edge on abilities and doubles their speed
          while swimming. If there are no open water pits on the encounter map,
          the water drains away at the end of the round.
~~~