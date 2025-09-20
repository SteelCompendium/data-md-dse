---
agility: 0
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '7'
file_basename: War Dog Tormentite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 3
intuition: 3
item_id: war-dog-tormentite
item_index: '393'
item_name: War Dog Tormentite
level: 5
might: 0
presence: 0
reason: 2
roles:
- Horde Hexer
scc:
- mcdm.monsters.v1:monster:war-dog-tormentite
scdc:
- 1.1.1:2:393
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '30'
type: monster
---

~~~ds-statblock
type: statblock
name: War Dog Tormentite
level: 5
roles:
  - Horde Hexer
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "7"
stamina: "30"
speed: 5
size: 1M
stability: 0
free_strike: 3
might: 0
agility: 0
reason: 2
intuition: 3
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Mark of Agony
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        tier1: 6 corruption damage
        tier2: 8 corruption damage; the target is marked (save ends)
        tier3: 9 corruption damage; the target is marked (save ends)
      - name: Effect
        effect: Strikes made against a target marked this way gain an edge.
          Additionally, whenever the tormentite takes damage, each target marked
          by them takes 3 damage.
  - type: feature
    feature_type: ability
    name: Vortex of Pain
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    usage: Main action
    distance: 4 cube within 10
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        tier1: 2 corruption damage
        tier2: 4 corruption damage
        tier3: 5 corruption damage; one ally in the area can end one effect on them that
          can be ended by a saving throw, and can give that effect to one target
      - name: Effect
        effect: The tormentite regains 2 Stamina for each creature targeted by this
          ability.
  - type: feature
    feature_type: trait
    name: Persistent Pain
    icon: ⭐️
    effects:
      - effect: From the start of the encounter, the tormentite takes 1 damage at the
          start of each of their turns.
  - type: feature
    feature_type: trait
    name: Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When the tormentite is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 2d6 damage to each adjacent enemy and object.
~~~