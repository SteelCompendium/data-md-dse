---
file_basename: Psionic Shard
file_dpath: Dynamic Terrain/Power Fixtures
item_id: psionic-shard-level-5-fortification-defender
item_index: '01'
item_name: Psionic Shard (Level 5 Fortification Defender)
scc:
- mcdm.monsters.v1:dynamic-terrain.power-fixture:psionic-shard-level-5-fortification-defender
scdc:
- 1.1.1:4.4:01
source: mcdm.monsters.v1
type: dynamic-terrain/power-fixture
---

~~~ds-featureblock
name: Psionic Shard
type: Fortification Defender
level: 5
ev: "7"
flavor: A massive humming crystal makes the air around it feel thick.
stamina: "40"
size: "2"
stats: []
features:
  - name: Deactivate
    icon: 🌀
    effects:
      - effect: The psionic shard must be completely destroyed.
  - name: Psionic Barrier
    icon: ⭐️
    effects:
      - effect: A psionic shard is attuned to one side in an encounter. While a psionic
          shard is intact, any damage dealt to each ally of the shard in the
          encounter is halved.
  - name: Psionic Pulse
    icon: ❗️
    keywords:
      - "-"
    type: Free triggered action
    distance: "-"
    target: "-"
    trigger: The shard is destroyed.
    effects:
      - effect: The shard releases a shockwave channeled through each creature affected
          by Psionic Barrier. Each ally in the encounter is dazed until the end
          of their next turn.
        name: Effect
~~~