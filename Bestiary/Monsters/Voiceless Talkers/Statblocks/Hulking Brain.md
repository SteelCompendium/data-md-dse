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
item_index: '335'
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
- 1.1.1:2:335
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 4
stamina: '180'
type: monster
---

~~~ds-statblock
type: statblock
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
features:
  - type: feature
    feature_type: ability
    name: Four-Way Grasp
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: Four creatures or objects
    effects:
      - roll: Power Roll + 3
        tier1: 7 damage
        tier2: 10 damage; A < 2 grabbed
        tier3: 11 damage; A < 3 grabbed
      - name: Special
        effect: The hulking brain can have up to four size 1 creatures grabbed.
      - cost: 2 Malice
        effect: The potency increases by 1.
  - type: feature
    feature_type: ability
    name: Cerebral Suplex
    icon: 🗡
    keywords:
      - Melee
      - Strike
    usage: Main action
    distance: Melee 1
    target: Each enemy
    effects:
      - name: Effect
        effect: A target must be grabbed by the hulking brain, and is no longer grabbed
          after the power roll is resolved.
      - roll: Power Roll + 3
        tier1: 7 damage; M < 1 3 damage
        tier2: 10 damage; M < 2 3 damage
        tier3: 13 damage; M < 3 6 damage
  - type: feature
    feature_type: ability
    name: Lumber
    icon: 👤
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The hulking brain shifts up to 4 squares, ignoring difficu terrain.
  - type: feature
    feature_type: ability
    name: Brawny Buffe
    icon: ❗️
    cost: 1 Malice
    keywords:
      - "-"
    usage: Free triggered action
    distance: Self
    target: Self
    trigger: An ally voiceless talker within 5 squares takes damage from an enemy
      ability.
    effects:
      - name: Effect
        effect: The hulking brain shifts adjacent to the ally and becomes the new target
          of the ability.
      - cost: 2 Malice
        effect: The enemy is knocked prone.
  - type: feature
    feature_type: trait
    name: Biceps to Spare
    icon: ⭐️
    effects:
      - effect: The hulking brain can carry up to four size 1 creatures they have
          grabbed, and takes no penalty to their speed while doing so.
  - type: feature
    feature_type: trait
    name: Psionic Conductor
    icon: ⭐️
    effects:
      - effect: Whenever a non-minion voiceless talker within 5 squares of the hulking
          brain uses a psionic ability, they can do so as if they were in the
          hulking brain's space.
~~~