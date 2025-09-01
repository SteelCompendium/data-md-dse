---
file_basename: Orc Malice Malice Features
file_dpath: Monsters/Orcs/Features
item_id: orc-malice-malice-features
item_index: '16'
item_name: Orc Malice Malice Features
scc:
- mcdm.monsters.v1:monster.feature:orc-malice-malice-features
scdc:
- 1.1.1:2.2:16
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Orc Malice Malice Features
flavor: At the start of any orc's turn, you can spend Malice to activate one of
  the following features.
stats: []
features:
  - name: Overwhelming March
    icon: ⭐️
    cost: 3 Malice
    effects:
      - effect: Each orc shifts up to their speed, moving through enemy spaces if they
          can. Each enemy passed through during this movement makes a **Might
          test**.
        t1: 6 damage; prone
        t2: 4 damage; prone
        t3: Push 2
  - name: Mohler Trench
    icon: 🔳
    cost: 5 Malice
    effects:
      - effect: An orc acting this turn summons 2 **mohlers** out of the ground, who dig
          a trench that is a 10 x 1 line within 10 squares when they appear. The
          trench is 2 squares deep and is difficult terrain. The trench can't be
          created directly underneath creatures.
  - name: Mohler Cavity
    icon: 🔳
    cost: 7 Malice
    effects:
      - effect: The ground shakes as a group of mohlers dig a 5 cube pit beneath an area
          where at least one creature is on the ground. The area is difficult
          terrain. Each orc in the area can shift into the nearest unoccupied
          space outside the pit before it is completed. Each nonorc in the area
          makes an **Agility test**.
        t1: 4 damage; the target falls; prone and can't stand (EoT)
        t2: 4 damage; the target falls
        t3: The target can shift into the nearest unoccupied space outside the pit.
~~~