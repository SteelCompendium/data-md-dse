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
item_index: '350'
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
- 1.1.1:2:350
size: '3'
source: mcdm.monsters.v1
speed: 3
stability: 5
stamina: '400'
type: monster
---

~~~ds-statblock
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
traits:
  - name: Solo Monster
    effects:
      - effect: At the end of each of their turns, the shambling mound can take 10
          damage to end one effect on them that can be ended by a saving throw.
          This damage can't be reduced in any way.
        name: End Effect
      - effect: The shambling mound can take two turns each round. They can't take turns
          consecutively.
        name: Solo Turns
  - name: Engulfing Sac
    effects:
      - effect: The shambling mound has a vegetative sack on their body where they carry
          engulfed creatures. The sack has 30 Stamina, damage immunity 5, and
          fire weakness 10. Destroying the sack frees creatures trapped by the
          shambling mound's Engulf ability. The shambling mound regrows a
          destroyed sack at the start of their next turn.
  - name: False Appearance
    effects:
      - effect: While the shambling mound remains motionless, they are indistinguishable
          from ordinary vegetation.
  - name: Frothing Flora
    effects:
      - effect: The area within 6 squares of the shambling mound is difficult terrain.
abilities:
  - name: Vine Lash
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 6
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        t1: 11 damage; A < 3 grabbed
        t2: 16 damage; A < 4 grabbed
        t3: 19 damage; grabbed
      - effect: The shambling mound can slide each target up to 6 squares.
        cost: 2 Malice
      - effect: Each target takes 7 poison damage.
        cost: 3 Malice
  - name: Seismic Slam
    icon: ❇️
    keywords:
      - Area
      - Weapon
    type: Main action
    distance: 6 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        t1: 4 damage; M < 2 dazed (save ends)
        t2: 6 damage; M < 3 dazed (save ends)
        t3: 7 damage; M < 4 dazed (save ends)
  - name: Engulf
    icon: 🗡
    cost: 2 Malice
    keywords:
      - Melee
    type: Main action
    distance: Melee 6
    target: One creature or object
    effects:
      - effect: The target must be size 1L or smaller. The shambling mound reaches out
          with writhing vines, and if the target has A < 3, they are engulfed
          into the shambling mound's sack. If the target is grabbed by the
          shambling mound, the potency increases by 1. An engulfed creature is
          restrained, takes 3 poison damage at the start of each turn, and can't
          take damage from abilities used from outside the sack. When the
          shambling mound moves, the engulfed creature moves with them. If the
          shambling mound dies or their sack is destroyed, each engulfed
          creature is freed and appears in an unoccupied space within 2 squares
          of the shambling mound.
        name: Effect
      - effect: The shambling mound can engulf one additional target for each 2 Malice
          spent.
        cost: 2+ Malice
  - name: Leech
    icon: 👤
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: Each creature engulfed by the shambling mound takes 5 poison damage. The
          shambling mound gains 5 temporary Stamina for each creature who takes
          damage this way.
        name: Effect
  - name: Tether Down
    icon: ❗️
    keywords:
      - Melee
    type: Triggered action
    distance: Melee 6
    target: The triggering creature
    trigger: A creature within distance willingly moves.
    effects:
      - roll: Power Roll + 4
        t1: 7 damage; M < 2 restrained (EoT)
        t2: 12 damage; M < 3 restrained (EoT)
        t3: 15 damage; M < 4 restrained (EoT)
  - name: Ravenous Overgrowth
    icon: ☠️
    cost: Villain Action 1
    keywords:
      - Area
      - Weapon
    type: "-"
    distance: 10 x 2 line within 1
    target: Each creature in the area
    effects:
      - roll: Power Roll + 4
        t1: 7 damage, pull 3
        t2: 12 damage; pull 4; the target has poison weakness 3 until the end of the
          encounter
        t3: 15 damage; pull 6; the target has poison weakness 5 until the end of the
          encounter
  - name: Composting
    icon: ☠️
    cost: Villain Action 2
    keywords:
      - Melee
    type: "-"
    distance: Melee 6
    target: Each enemy
    effects:
      - effect: The shambling mound uses Engulf against each target without spending
          Malice.
        name: Effect
  - name: Exposed Crux
    icon: ☠️
    cost: Villain Action 3
    keywords:
      - Melee
    type: "-"
    distance: Self
    target: Self
    effects:
      - effect: The shambling mound rips themself apart, exposing the crux of magic
          holding them together. The distance of the shambling mound's melee
          abilities increases to melee 10, the creature has a double edge on
          power rolls, and strikes made against them gain an edge.
        name: Effect
~~~