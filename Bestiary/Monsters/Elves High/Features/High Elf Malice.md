---
file_basename: High Elf Malice
file_dpath: Monsters/Elves High/Features
item_id: high-elf-malice-malice-features
item_index: '14'
item_name: High Elf Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:high-elf-malice-malice-features
scdc:
- 1.1.1:2.2:14
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: High Elf Malice
type: Malice Features
flavor: At the start of any high elf's turn, you can spend Malice to activate
  one of the following features.
stats: []
features:
  - name: Chaincast
    icon: 🌀
    cost: 3 Malice
    effects:
      - effect: Until the end of the round, whenever a high elf uses a magic ability,
          they can use it as if they were occupying the square of another high
          elf on the encounter map to whom they have line of effect.
  - name: \*\*Gift From an Accursed Tome
    icon: 🔳
    cost: 5 Malice
    keywords:
      - Area
      - Magic
    type: Main action
    distance: 5 x 1 line within 1
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: "The high elf chooses a damage type and condition from one of the
          following combinations: cold damage and slowed, poison damage and
          weakened, or corruption damage and frightened."
      - roll: Power Roll + 2
        t1: 5 damage; R < 1 chosen condition (save ends)
        t2: 9 damage; R < 2 chosen condition (save ends)
        t3: 12 damage; R < 3 chosen condition (save ends)
      - effect: This ability can't be used by a minion.
        name: Special
  - name: In Defiance of Time
    icon: 🌀
    cost: 7 Malice
    effects:
      - effect: Until the end of the round, each high elf in the encounter gains a +4
          bonus to speed, and whenever a high elf uses an ability against an
          enemy, each high elf adjacent to that enemy can make a free strike
          against them.
~~~