---
file_basename: Chimera Malice
file_dpath: Monsters/Chimera/Features
item_id: chimera-malice-malice-features
item_index: '01'
item_name: Chimera Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:chimera-malice-malice-features
scdc:
- 1.1.1:2.2:01
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
name: Chimera Malice
type: Malice Features
flavor: At the start of a chimera's turn, you can spend Malice to activate one
  of the following features.
features:
  - name: Defensive Snapping
    icon: ⭐️
    cost: 3 Malice
    effects:
      - effect: The chimera takes up a defensive stance. Until the start of their next
          turn, the chimera can make a free strike against each enemy who comes
          within 2 squares of them.
  - name: Solo Action
    icon: ☠️
    cost: 5 Malice
    effects:
      - effect: The chimera takes an additional main action on their turn. They can use
          this feature even if they are dazed.
  - name: Unstable Terrain
    icon: 🔳
    cost: 5 Malice
    effects:
      - effect: The chimera shakes the ground, causing an eruption of loose rocks and
          debris that creates three size 2 stone objects anywhere on the
          encounter map. Each creature adjacent to one or more objects when they
          appear who has A < 2 takes 5 damage.
  - name: Ashen Clouds
    icon: 🌀
    cost: 7 Malice
    effects:
      - effect: Until the start of the chimera's next turn, all areas of the encounter
          map are shrouded in a thick cloud of ash. All creatures and objects on
          the map have concealment that the chimera ignores. Additionally, each
          enemy in the cloud who has I < 1 has line of effect only within 3
          squares. The potency of this feature increases by 1 each time it's
          used.
~~~