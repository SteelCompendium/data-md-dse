---
file_basename: Manticore Malice
file_dpath: Monsters/Manticores/Features
item_id: manticore-malice-malice-features
item_index: '55'
item_name: Manticore Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:manticore-malice-malice-features
scdc:
- 1.1.1:2.2:55
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Manticore Malice
type: Malice Features
flavor: At the start of any manticore's turn, you can spend Malice to activate
  one of the following features.
features:
  - name: Uncanny Mimicry
    icon: 🌀
    cost: 3 Malice
    effects:
      - effect: The manticore uses their mimicry in an attempt to unnerve one creature
          within their line of effect. If the target has R < 4, they take a bane
          on power rolls against the manticore (save ends). Each time this
          feature is used against the same target during the encounter, its
          potency decreases by 2.
  - name: Solo Action
    icon: ☠️
    cost: 5 Malice
    effects:
      - effect: The manticore takes an additional main action on their turn. They can
          use this feature even if they are dazed.
  - name: Desperate Howl
    icon: 🌀
    cost: 5 Malice
    effects:
      - effect: The manticore lets out an unnerving cry. Each enemy within the
          manticore's line of effect makes an **Intuition test**.
        t1: Frightened (save ends)
        t2: Frightened (EoT)
        t3: No effect.
  - name: Barrage of Barbs
    icon: ❇️
    cost: 7 Malice
    effects:
      - effect: The manticore sprays tail spikes across the ground within 5 squares of
          them. Each enemy in that area who has A < 3 is bleeding (save ends).
          Additionally, the area is difficult terrain, and any enemy takes 3
          poison damage for each square of the area they enter. An enemy who
          takes 9 poison damage this way on one turn is weakened until the end
          of the encounter.
~~~