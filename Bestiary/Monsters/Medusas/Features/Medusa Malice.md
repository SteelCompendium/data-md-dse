---
file_basename: Medusa Malice
file_dpath: Monsters/Medusas/Features
item_id: medusa-malice-malice-features
item_index: '30'
item_name: Medusa Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:medusa-malice-malice-features
scdc:
- 1.1.1:2.2:30
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Medusa Malice
type: Malice Features
flavor: At the start of a medusa's turn, you can spend Malice to activate one of
  the following features.
stats: []
features:
  - name: Weakening Glare
    icon: 🏹
    cost: 4 Malice
    keywords:
      - "- Magic"
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 10
    target: One creature
    effects:
      - roll: Power Roll + 4
        t1: 6 damage; weakened (EoT)
        t2: 10 damage; weakened (EoT)
        t3: 12 damage; weakened (save ends)
  - name: Solo Action
    icon: ☠️
    cost: 5 Malice
    effects:
      - effect: The medusa takes an additional main action on their turn. They can use
          this feature even if they are dazed.
  - name: Ssstop and Lisssten
    icon: 🏹
    cost: 5 Malice
    keywords:
      - Magic
      - Ranged
    type: Main action
    distance: Ranged 10
    target: Three creatures
    effects:
      - roll: Power Roll + 4
        t1: I < 2 the target is charmed
        t2: I < 3 the target is charmed
        t3: I < 4 the target is charmed
      - effect: At a time of the medusa's choosing, a charmed creature moves up to their
          speed and makes a free strike against an enemy of the medusa's choice
          as a free triggered action. The creature is then no longer charmed.
        name: Effect
  - name: Shatter Victims
    icon: 🔳
    cost: 7 Malice
    effects:
      - effect: The medusa causes three stone statues within 10 squares of them to each
          shatter in a 2-cube explosion. Each enemy in one of those areas makes
          a **Might test**. An enemy restrained or slowed by the medusa's
          Petrify ability has a double bane on the test.
        t1: 12 damage; vertical push 3; bleeding (save ends)
        t2: 10 damage; vertical push 3
        t3: 6 damage
~~~