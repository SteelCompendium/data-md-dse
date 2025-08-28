---
file_basename: Troll Malice
file_dpath: Monsters/Trolls/Features
item_id: troll-malice-malice-features
item_index: '54'
item_name: Troll Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:troll-malice-malice-features
scdc:
- 1.1.1:2.2:54
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Troll Malice
type: Malice Features
flavor: At the start of any troll's turn, you can spend Malice to activate one
  of the following features.
stats: []
features:
  - name: Foul Spew
    icon: 🔳
    cost: 3 Malice
    effects:
      - effect: One troll acting this turn spews out a half-digested meal in a 5 x 1
          line within 1 square of them. Each troll in the area regains 3
          Stamina. Each enemy in the area makes a **Might test**.
        t1: 12 acid damage; dazed (EoT)
        t2: 10 acid damage; weakened (EoT)
        t3: 6 acid damage
  - name: Emergency Meal
    icon: 🗡
    cost: 5 Malice
    effects:
      - effect: Each troll in the encounter can make a free strike against a creature
          adjacent to them, and regains Stamina equal to the damage dealt.
  - name: Bloody Banquet
    icon: ❇️
    cost: 7 Malice
    effects:
      - effect: Each winded troll in the encounter disgorges the contents of their
          stomach onto the ground around them, creating a 1 burst of foul
          vomitus that lasts until the end of the encounter. Each non-troll who
          enters this area for the first time in a round or starts their turn
          there takes 5 acid damage. Each troll in the area has a double edge on
          power rolls.
~~~