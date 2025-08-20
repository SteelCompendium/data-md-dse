---
agility: -2
ancestry:
- Construct
- Servok
- Soulless
- Valok
ev: '48'
file_basename: Servok War Engine
file_dpath: Monsters/Valok/Statblocks
free_strike: 0
intuition: -1
item_id: servok-war-engine
item_index: '329'
item_name: Servok War Engine
level: 10
might: 5
presence: -5
reason: -4
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:servok-war-engine
scdc:
- 1.1.1:2:329
size: '3'
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '2608'
type: monster
---

```ds-statblock
name: Servok War Engine
level: 10
roles:
  - Elite Brute
ancestry:
  - Construct
  - Servok
  - Soulless
  - Valok
ev: "48"
stamina: "2608"
speed: 5
size: "3"
stability: 1
free_strike: 0
might: 5
agility: -2
reason: -4
intuition: -1
presence: -5
traits:
  - name: Servok Siege Machine
    effects:
      - effect: The war engine ignores difficult terrain, and their abilities deal an
          extra 15 damage to objects.
  - name: Crafted to Perfection
    effects:
      - effect: The war engine's shape can't be changed by any external effect
  - name: Valiar Might
    effects:
      - effect: While the war engine isn't bleeding, weakened, or winded, any power roll
          made against them is automatically a tier 1 outcome. A critical hit
          still grants its additional main action.
abilities:
  - name: Blade Rake
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 3
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 5
        t1: 15 damage
        t2: 21 damage; pull 3
        t3: 25 damage; pull 6
  - name: Prismacore Cannon
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 20
    target: One creature or object
    effects:
      - roll: Power Roll + 5
        t1: 22 damage
        t2: 29 damage; I < 4 dazed (save ends)
        t3: 34 damage; I < 5 dazed (save ends)
      - effect: This damage can't be reduced in any way. This ability can't be used
          again until the start of the next round.
  - name: Destructive Rollout
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The war engine moves up to their speed in a straight line, automatically
          destroying mundane size 1 objects or walls in their path. The first
          time the war engine moves through a creature's space during this
          movement, that creature can choose to either fall prone or take 10
          damage.
  - name: Burning Oil
    cost: 3 Malice
    keywords:
      - Area
    type: Maneuver
    distance: 20 x 1 line within 1
    target: Each enemy and object in the area
    effects:
      - effect: >-
          Each target makes an Agility test.

          - **≤11:** 16 fire damage; the target is burning (save ends

          - **12-16:** 12 fire damage; the target is burning (EoT

          - **17+:** 8 fire damage

          A burning creature takes 1d6 fire damage at the start of each of their
          turns. A burning object takes 1d6 fire damage at the end of each
          round. Additionally, the area is burning until the end of the
          encounter. While the area is burning, it is difficult terrain and any
          enemy takes 3 fire damage for each square of the area they enter.
  - name: Quick Blast
    cost: 1 Malice
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Free triggered action
    distance: Ranged 20
    target: One creature or object
    trigger: The target deals damage to the war engine.
    effects:
      - roll: Power Roll + 5
        t1: 8 damage; push 2
        t2: 12 damage; push 5
        t3: 16 damage; push 8
      - effect: This damage can't be reduced in any way.
```