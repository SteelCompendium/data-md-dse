---
agility: 1
ancestry:
- Horror
- Voiceless Talker
ev: '32'
file_basename: Hulking Brain
file_dpath: Monsters/Voiceless Talkers/Statblocks
free_strike: 7
intuition: -2
item_id: hulking-brain
item_index: '337'
item_name: Hulking Brain
level: 6
might: 3
presence: 0
reason: -2
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:hulking-brain
scdc:
- 1.1.1:2:337
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 4
stamina: '180'
type: monster
---

```ds-statblock
name: Hulking Brain
level: 6
roles:
  - Elite Brute
ancestry:
  - Horror
  - Voiceless Talker
ev: "32"
stamina: "180"
speed: 5
size: 1L
stability: 4
free_strike: 7
might: 3
agility: 1
reason: -2
intuition: -2
presence: 0
traits:
  - name: Biceps to Spare
    effects:
      - effect: The hulking brain can carry up to four size 1 creatures they have
          grabbed, and takes no penalty to their speed while doing so.
  - name: Psionic Conductor
    effects:
      - effect: Whenever a non-minion voiceless talker within 5 squares of the hulking
          brain uses a psionic ability, they can do so as if they were in the
          hulking brain's space.
abilities:
  - name: Four-Way Grasp
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: Four creatures or objects
    effects:
      - roll: Power Roll + 3
        t1: 7 damage
        t2: 10 damage; A < 2 grabbed
        t3: 11 damage; A < 3 grabbed
      - effect: The hulking brain can have up to four size 1 creatures grabbed.
        name: Special
      - effect: The potency increases by 1.
        cost: 2 Malice
  - name: Cerebral Suplex
    keywords:
      - Melee
      - Strike
    type: Main action
    distance: Melee 1
    target: Each enemy
    effects:
      - effect: A target must be grabbed by the hulking brain, and is no longer grabbed
          after the power roll is resolved
      - roll: Power Roll + 3
        t1: 7 damage; M < 1 3 damage
        t2: 10 damage; M < 2 3 damage
        t3: 13 damage; M < 3 6 damage
  - name: Lumber
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The hulking brain shifts up to 4 squares, ignoring difficu terrain.
  - name: Brawny Buffe
    cost: 1 Malice
    keywords:
      - "-"
    type: Free triggered action
    distance: Self
    target: Self
    trigger: An ally voiceless talker within 5 squares takes damage from an enemy
      ability.
    effects:
      - effect: The hulking brain shifts adjacent to the ally and becomes the new target
          of the ability.
      - effect: The enemy is knocked prone.
        cost: 2 Malice
```