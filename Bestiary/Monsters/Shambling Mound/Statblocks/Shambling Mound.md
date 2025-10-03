---
agility: -1
ancestry:
- Plant
- Shambling Mound
ev: '84'
file_basename: Shambling Mound
file_dpath: Monsters/Shambling Mound/Statblocks
free_strike: 7
intuition: 1
item_id: shambling-mound
item_index: '348'
item_name: Shambling Mound
level: 5
might: 4
presence: 0
reason: 0
roles:
- Solo
scc:
- mcdm.monsters.v1:monster:shambling-mound
scdc:
- 1.1.1:2:348
size: '3'
source: mcdm.monsters.v1
speed: 3
stability: 5
stamina: '400'
type: monster
---

~~~ds-statblock
type: statblock
name: Shambling Mound
level: 5
roles:
  - Solo
ancestry:
  - Plant
  - Shambling Mound
ev: "84"
stamina: "400"
speed: 3
size: "3"
stability: 5
free_strike: 7
might: 4
agility: -1
reason: 0
intuition: 1
presence: 0
features:
  - type: feature
    feature_type: trait
    name: Solo Monster
    icon: ☠️
    effects:
      - name: End Effect
        effect: At the end of each of their turns, the shambling mound can take 10
          damage to end one effect on them that can be ended by a saving throw.
          This damage can't be reduced in any way.
      - name: Solo Turns
        effect: The shambling mound can take two turns each round. They can't take turns
          consecutively.
  - type: feature
    feature_type: trait
    name: Engulfing Sac
    icon: ⭐️
    effects:
      - effect: The shambling mound has a vegetative sack on their body where they carry
          engulfed creatures. The sack has 30 Stamina, damage immunity 5, and
          fire weakness 10. Destroying the sack frees creatures trapped by the
          shambling mound's Engulf ability. The shambling mound regrows a
          destroyed sack at the start of their next turn.
  - type: feature
    feature_type: ability
    name: Vine Lash
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 6
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        tier1: 11 damage; A < 3 grabbed
        tier2: 16 damage; A < 4 grabbed
        tier3: 19 damage; grabbed
      - cost: 2 Malice
        effect: The shambling mound can slide each target up to 6 squares.
      - cost: 3 Malice
        effect: Each target takes 7 poison damage.
  - type: feature
    feature_type: ability
    name: Seismic Slam
    icon: ❇️
    keywords:
      - Area
      - Weapon
    usage: Main action
    distance: 6 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        tier1: 4 damage; M < 2 dazed (save ends)
        tier2: 6 damage; M < 3 dazed (save ends)
        tier3: 7 damage; M < 4 dazed (save ends)
  - type: feature
    feature_type: ability
    name: Engulf
    icon: 🗡
    cost: 2 Malice
    keywords:
      - Melee
    usage: Main action
    distance: Melee 6
    target: One creature or object
    effects:
      - name: Effect
        effect: The target must be size 1L or smaller. The shambling mound reaches out
          with writhing vines, and if the target has A < 3, they are engulfed
          into the shambling mound's sack. If the target is grabbed by the
          shambling mound, the potency increases by 1. An engulfed creature is
          restrained, takes 3 poison damage at the start of each turn, and can't
          take damage from abilities used from outside the sack. When the
          shambling mound moves, the engulfed creature moves with them. If the
          shambling mound dies or their sack is destroyed, each engulfed
          creature is freed and appears in an unoccupied space within 2 squares
          of the shambling mound.
      - cost: 2+ Malice
        effect: The shambling mound can engulf one additional target for each 2 Malice
          spent.
  - type: feature
    feature_type: ability
    name: Leech
    icon: 👤
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: Each creature engulfed by the shambling mound takes 5 poison damage. The
          shambling mound gains 5 temporary Stamina for each creature who takes
          damage this way.
  - type: feature
    feature_type: ability
    name: Tether Down
    icon: ❗️
    keywords:
      - Melee
    usage: Triggered action
    distance: Melee 6
    target: The triggering creature
    trigger: A creature within distance willingly moves.
    effects:
      - roll: Power Roll + 4
        tier1: 7 damage; M < 2 restrained (EoT)
        tier2: 12 damage; M < 3 restrained (EoT)
        tier3: 15 damage; M < 4 restrained (EoT)
  - type: feature
    feature_type: trait
    name: False Appearance
    icon: ⭐️
    effects:
      - effect: While the shambling mound remains motionless, they are indistinguishable
          from ordinary vegetation.
  - type: feature
    feature_type: trait
    name: Frothing Flora
    icon: ⭐️
    effects:
      - effect: The area within 6 squares of the shambling mound is difficult terrain.
  - type: feature
    feature_type: ability
    name: Ravenous Overgrowth
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
      - Weapon
    usage: "-"
    distance: 10 x 2 line within 1
    target: Each creature in the area
    effects:
      - roll: Power Roll + 4
        tier1: 7 damage, pull 3
        tier2: 12 damage; pull 4; the target has poison weakness 3 until the end of the
          encounter
        tier3: 15 damage; pull 6; the target has poison weakness 5 until the end of the
          encounter
  - type: feature
    feature_type: ability
    name: Composting
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - Melee
    usage: "-"
    distance: Melee 6
    target: Each enemy
    effects:
      - name: Effect
        effect: The shambling mound uses Engulf against each target without spending
          Malice.
  - type: feature
    feature_type: ability
    name: Exposed Crux
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Melee
    usage: "-"
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The shambling mound rips themself apart, exposing the crux of magic
          holding them together. The distance of the shambling mound's melee
          abilities increases to melee 10, the creature has a double edge on
          power rolls, and strikes made against them gain an edge.
~~~