---
file_basename: Omen Dragon Malice
file_dpath: Monsters/Dragons/Features
item_id: omen-dragon-malice-malice-features
item_index: '52'
item_name: Omen Dragon Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:omen-dragon-malice-malice-features
scdc:
- 1.1.1:2.2:52
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Omen Dragon Malice
type: Malice Features
flavor: At the start of an omen dragon's turn, you can spend Malice to activate
  one of the following features.
features:
  - name: Black Skies
    icon: ⭐️
    cost: 3 Malice
    effects:
      - effect: The dragon expands their wings to create a shroud of shadow. Until the
          start of the dragon's next turn, any strike made against them takes a
          bane.
  - name: Rise and Fall
    icon: ❇️
    cost: 5 Malice
    effects:
      - effect: The dragon flies up to 10 squares and carries fated souls with them.
          Each creature in the area of the dragon's Stagnant Wyrmscale Aura
          trait makes a **Presence test**.
        t1: Vertical pull 10
        t2: Vertical pull 6
        t3: Vertical pull 4
  - name: Solo Action
    icon: ☠️
    cost: 5 Malice
    effects:
      - effect: The dragon takes an additional main action on their turn. They can use
          this feature even if they are dazed.
  - name: Burn It Right Down
    icon: 🌀
    cost: 10 Malice
    effects:
      - effect: Each edge of the encounter map burns with intangible purple flames until
          the end of the encounter. The flames expand by 1 square at the end of
          every turn. Any enemy takes 5 corruption damage for each square of
          flames they enter.
~~~