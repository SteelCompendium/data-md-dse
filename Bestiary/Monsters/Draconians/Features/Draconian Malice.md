---
file_basename: Draconian Malice
file_dpath: Monsters/Draconians/Features
item_id: draconian-malice-malice-features
item_index: 09
item_name: Draconian Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:draconian-malice-malice-features
scdc:
- 1.1.1:2.2:09
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Draconian Malice
type: Malice Features
flavor: At the start of any draconian's turn, you can spend Malice to activate
  one of the following features.
stats: []
features:
  - name: Guarding Gale
    icon: 👤
    cost: 3 Malice
    effects:
      - effect: A draconian acting this turn flaps their wings and creates a mighty
          gale. Each creature adjacent to the draconian is pushed up to 4
          squares, and if they have M < 2, they are knocked prone.
  - name: Breath Weapon
    icon: 🔳
    cost: 5 Malice
    keywords:
      - Area
      - Magic
    type: Main action
    distance: 4 x 2 line within 1
    target: Each enemy in the area
    effects:
      - name: Special
        effect: The damage dealt by this ability matches a damage type the draconian has
          immunity to.
      - roll: Power Roll + 3
        t1: 6 damage
        t2: 10 damage
        t3: 13 damage
  - name: Scaleshatter Burst
    icon: ❇️
    cost: 7 Malice
    keywords:
      - Area
      - Magic
    type: Free maneuver
    distance: 2 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        t1: 7 damage
        t2: 13 damage
        t3: 16 damage
      - effect: The draconian's scales shatter from battle damage. The draconian has
          damage weakness 5 but can take two turns per round until the end of
          the encounter.
        name: Effect
~~~