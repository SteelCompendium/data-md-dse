---
agility: 1
ancestry:
- Bugbear
- Fey
- Goblin
- Humanoid
ev: '16'
file_basename: Bugbear Channeler
file_dpath: Monsters/Bugbears/Statblocks
free_strike: 5
intuition: 2
item_id: bugbear-channeler
item_index: '290'
item_name: Bugbear Channeler
level: 2
might: 1
presence: 2
reason: 2
roles:
- Elite Controller
scc:
- mcdm.monsters.v1:monster:bugbear-channeler
scdc:
- 1.1.1:2:290
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '60'
type: monster
---

```ds-statblock
name: Bugbear Channeler
level: 2
roles:
  - Elite Controller
ancestry:
  - Bugbear
  - Fey
  - Goblin
  - Humanoid
ev: "16"
stamina: "60"
speed: 5
size: 1L
stability: 0
free_strike: 5
might: 1
agility: 1
reason: 2
intuition: 2
presence: 2
traits: []
abilities:
  - name: Shadow Drag
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged. Strike
    type: Main Action
    distance: Ranged 8
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        t1: 7 damage; pull 2
        t2: 10 damage; pull 3
        t3: 13 damage; pull 4
      - effect: Each target must be on the ground, and each square a target is pulled
          through is difficult terrain for enemies.
  - name: Blistering Element
    keywords:
      - Area
      - Magic
    type: Main Action
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - effect: "The channeler chooses one of the following damage types: acid, cold,
          corruption, fire, or poison."
      - roll: Power Roll + 2
        t1: 2 damage; M < 0 bleeding (save ends)
        t2: 3 damage; M < 1 bleeding (save ends)
        t3: 4 damage; M < 2 bleeding (save ends)
  - name: Twist Shape
    cost: 5 Malice
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main Action
    distance: Ranged 5
    target: One creature
    effects:
      - roll: Power Roll + 2
        t1: 5 corruption damage; P < 0 slowed (save ends)
        t2: 8 corruption damage; P < 1 the target is shapechanged (save ends)
        t3: 11 corruption damage; P < 2 the target is shapechanged (save ends)
      - effect: A shapechanged creature is slowed and has fire weakness 10 as their
          limbs stretch and their skin becomes paper thin.
  - name: Throw
    keywords:
      - Melee
      - Strike
    type: Maneuver
    distance: Melee 1
    target: One creature or object
    effects:
      - effect: The target must be grabbed by the channeler.
        name: Special
      - effect: The target is vertical pushed up to 3 squares. An ally doesn't take
          damage from being force moved this way.
  - name: Catcher
    keywords:
      - Melee
    type: Free triggered action
    distance: Melee 1
    target: The triggering creature or object
    trigger: A size 1 creature or object is force moved within distance, or a size 1
      ally willingly moves within distance.
    effects:
      - effect: The target is grabbed by the channeler.
  - name: Shadow Veil
    keywords:
      - Magic
      - Ranged
    type: Triggered action
    distance: Ranged 5
    target: The triggering ally
    trigger: An ally within distance takes damage.
    effects:
      - effect: The target is wrapped in shadow and halves the damage. The target can't
          be targeted by strikes until the start of their next turn.
```