---
file_basename: Arixx Malice
file_dpath: Monsters/Arixx/Features
item_id: arixx-malice-malice-features
item_index: '30'
item_name: Arixx Malice (Malice Features)
scc:
- mcdm.monsters.v1:monster.feature:arixx-malice-malice-features
scdc:
- 1.1.1:2.2:30
source: mcdm.monsters.v1
type: monster/feature
---

~~~ds-featureblock
type: featureblock
featureblock_type: Malice Features
name: Arixx Malice
flavor: At the start of an arixx's turn, you can spend Malice to activate one of
  the following features.
features:
  - type: feature
    feature_type: trait
    name: Burning Maw
    icon: 👤
    cost: 3 Malice
    effects:
      - effect: The arixx dribbles acid over their mandibles, causing the next strike
          they make to gain an edge and deal an extra 3 acid damage.
  - type: feature
    feature_type: trait
    name: Geyser
    icon: 🔳
    cost: 5 Malice
    effects:
      - effect: The arixx's underground tunnels swell with pressure, causing a sudden
          influx of hot gas to burst from a 3-square-by-3-square area anywhere
          on the surface. Each enemy in the area makes an **Agility test**.
        tier1: 4 damage; vertical push 5
        tier2: 4 damage; vertical push 3
        tier3: The target shifts to the nearest unoccupied space outside the area.
  - type: feature
    feature_type: trait
    name: Solo Action
    icon: ☠️
    cost: 5 Malice
    effects:
      - effect: The arixx takes an additional main action on their turn. They can use
          this feature even if they are dazed.
  - type: feature
    feature_type: trait
    name: Earth Sink
    icon: 🌀
    cost: 7 Malice
    effects:
      - effect: The encounter map suddenly quakes, then begins to sink. Each creature on
          the ground who has A < 1 is knocked prone. Until the end of the
          encounter, each creature who starts their turn on the ground and can't
          burrow must spend 1 additional square of movement to leave their
          starting position, or 2 squares if they start their turn prone or
          underground. A creature who starts and ends their turn in the same
          space on the ground and can't burrow sinks 1 square into the ground.
~~~