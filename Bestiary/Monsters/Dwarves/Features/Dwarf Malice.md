---
file_basename: Dwarf Malice
file_dpath: Monsters/Dwarves/Features
item_id: dwarf-malice-malice-features
item_index: '53'
item_name: Dwarf Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:dwarf-malice-malice-features
scdc:
- 1.1.1:2.2:53
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Dwarf Malice
type: Malice Features
flavor: At the start of any dwarf's turn, you can spend Malice to activate one
  of the following features.
stats: []
features:
  - name: Breaching Charge
    icon: 👤
    cost: 3 Malice
    effects:
      - effect: A dwarf can destroy one adjacent object or square of wall for each 3
          Malice spent. Each enemy adjacent to the destroyed object or square
          takes the object's Stamina in damage (3 for wood, 6 for stone, or 9
          for metal).
  - name: Rappelling Barrage
    icon: ⭐️
    cost: 5 Malice
    effects:
      - effect: Each dwarf acting this turn can automatically climb at full speed while
          moving. At any point during this movement, they can make a free
          strike.
  - name: Snaring Line
    icon: 🔳
    cost: 7 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    type: Main action
    distance: 10 x 1 line within 10
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: Each target makes an **Agility test**.
        t1: 8 damage; restrained (EoT)
        t2: 6 damage; slowed (EoT)
        t3: No effect.
      - effect: The snaring line remains until the end of the encounter. Any enemy who
          moves into the area for the first time in a round or starts their turn
          there must make the test.
      - effect: This ability can't be used by a minion.
        name: Special
~~~