---
file_basename: Griffon Malice
file_dpath: Monsters/Griffons/Features
item_id: griffon-malice-malice-features
item_index: '07'
item_name: Griffon Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:griffon-malice-malice-features
scdc:
- 1.1.1:2.2:07
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Griffon Malice
type: Malice Features
flavor: At the start of any griffon's turn, you can spend Malice to activate one
  of the following features.
stats: []
features:
  - name: Swoop
    icon: 👤
    cost: 3 Malice
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The griffon flies up to their speed, and can make a free strike against
          each creature who makes an opportunity attack against them during this
          movement.
        name: Effect
  - name: Piercing Cry
    icon: ❇️
    cost: 5 Malice
    effects:
      - effect: A griffon acting this turn unleashes a hideous screech at one enemy
          within 5 squares of them, forcing that creature to make an **Intuition
          test**.
        t1: Frightened (save ends)
        t2: Frightened (EoT)
        t3: No effect.
  - name: Wildwinds
    icon: 🌀
    cost: 10 Malice
    effects:
      - effect: Winds bluster and blow across the encounter map. Until the end of the
          encounter, each creature who can't fly or isn't mounted on a flying
          creature takes a −3 penalty to stability, and any forced movement
          effect targeting such a creature moves them an additional 5 squares.
~~~