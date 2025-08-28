---
file_basename: Wode Elf Malice
file_dpath: Monsters/Elves Wode/Features
item_id: wode-elf-malice-malice-features
item_index: '26'
item_name: Wode Elf Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:wode-elf-malice-malice-features
scdc:
- 1.1.1:2.2:26
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Wode Elf Malice
type: Malice Features
flavor: At the start of any wode elf's turn, you can spend Malice to activate
stats:
  - name: ≤11
    value: 8 damage; restrained (save ends)
  - name: 12-16
    value: Restrained (EoT)
  - name: 17+
    value: No effect.
features:
  - name: Forest Network
    icon: ⭐️
    cost: 3 Malice
    effects:
      - effect: Each wode elf who ends this turn hidden can shift up to their speed
          while remaining hidden.
  - name: Punishing Regrowth
    icon: ⭐️
    cost: 5 Malice
    effects:
      - effect: Until the end of the round, each wode elf gains an edge on abilities,
          and their strikes can slide a target up to 2 squares in addition to
          their usual effects. If a strike already imposes forced movement, this
          slide happens after that forced movement. A creature force moved by a
          wode elf's strike who ends this forced movement in difficult terrain
          is restrained until the end of their next turn.
  - name: Vines Everywhere
    icon: 🌀
    cost: 7 Malice
    effects:
      - effect: Vines rapidly grow across the entire encounter map. Each enemy in the
          encounter makes an **Agility test**.
~~~