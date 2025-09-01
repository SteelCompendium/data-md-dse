---
file_basename: Angulotl Malice
file_dpath: Monsters/Angulotls/Features
item_id: angulotl-malice-malice-features
item_index: '32'
item_name: Angulotl Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:angulotl-malice-malice-features
scdc:
- 1.1.1:2.2:32
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Angulotl Malice
type: Malice Features
flavor: At the start of any angulotl's turn, you can spend Malice to activate
  one of the following features.
stats: []
features:
  - name: Leapfrog
    icon: ⭐️
    cost: 3 Malice
    effects:
      - effect: Until the end of the round, when an angulotl moves through an inactive
          angulotl's space, the inactive angulotl can use a free triggered
          action to jump 3 squares.
  - name: Resonating Croak
    icon: ❇️
    cost: 5 Malice
    effects:
      - effect: Each angulotl in the encounter puffs out their throat and starts loudly
          droning. Any non-angulotl adjacent to an angulotl makes an **Intuition
          test.**
        t1: 5 sonic damage; slowed (EoT)
        t2: 4 sonic damage
        t3: No effect.
  - name: Rainfall
    icon: 🌀
    cost: 7 Malice
    effects:
      - effect: An angulotl calls clouds to cover the encounter map and unleash rain
          until the end of the round. Any creature or object that is exposed to
          the sky is wet until the end of the encounter.
~~~