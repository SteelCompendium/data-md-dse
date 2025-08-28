---
file_basename: The Chronal Hypercube
file_dpath: Dynamic Terrain/Supernatural Objects
item_id: the-chronal-hypercube-level-3-relic-controller
item_index: '02'
item_name: The Chronal Hypercube (Level 3 Relic Controller)
scc:
- mcdm.monsters.v1:dynamic-terrain.supernatural-object:the-chronal-hypercube-level-3-relic-controller
scdc:
- 1.1.1:4.6:02
source: mcdm.monsters.v1
type: dynamic-terrain/supernatural-object
---

~~~ds-featureblock
name: The Chronal Hypercube
type: Relic Controller
level: 3
ev: "20"
flavor: This unnatural object twists space around it in a reflection of its own
  unnatural form.
stamina: "80"
size: 1M
stats: []
features:
  - name: Deactivate
    icon: 🌀
    effects:
      - effect: A creature who has the Psionics skill can deactivate and take control of
          the chronal hypercube by making a **Reason test** while within 10
          squares of the hypercube.
        t1: The creature takes 1d6 psychic damage.
        t2: The creature fails to deactivate the hypercube.
        t3: The hypercube teleports adjacent to the creature at the start of the next
          round and becomes an ally to the creature and their allies.
  - name: Dimensional Flicker
    icon: ⭐️
    effects:
      - effect: At the start of each round while the hypercube is present, roll a d10.
          On a 7 or higher, the hypercube teleports to a square of one ally's
          choice within 10 squares and is hidden. While the hypercube is hidden,
          Psionics is the only skill that can be applied to a test made to find
          it.
  - name: Chronal Superhighway
    icon: ⭐️
    effects:
      - effect: Any ally within 10 squares of the hypercube can teleport when they move.
          An ally who teleports gains an edge on the next power roll they make.
~~~