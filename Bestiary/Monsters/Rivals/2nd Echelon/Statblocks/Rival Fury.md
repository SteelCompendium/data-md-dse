---
agility: 2
ancestry:
- Humanoid
- Rival
ev: '28'
file_basename: Rival Fury
file_dpath: Monsters/Rivals/2nd Echelon/Statblocks
free_strike: 7
intuition: 0
item_id: rival-fury
item_index: '15'
item_name: Rival Fury
level: 5
might: 3
presence: 1
reason: 0
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:rival-fury
scdc:
- 1.1.1:2:15
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 3
stamina: '160'
type: monster
---

~~~ds-statblock
type: statblock
name: Rival Fury
level: 5
roles:
  - Elite Brute
ancestry:
  - Humanoid
  - Rival
ev: "28"
stamina: "160"
speed: 5
size: 1M
stability: 3
free_strike: 7
might: 3
agility: 2
reason: 0
intuition: 0
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Thunderous Slam
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        tier1: 10 damage; push 2
        tier2: 15 damage; push 3
        tier3: 18 damage; push 4
      - cost: 2 Malice
        effect: Each target who has M < 2 is slowed (save ends).
  - type: feature
    feature_type: ability
    name: Roughed Up
    icon: 🗡
    cost: 3 Malice
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature
    effects:
      - roll: Power Roll + 3
        tier1: 11 damage; M < 1 grabbed
        tier2: 16 damage; M < 2 grabbed
        tier3: 21 damage; M < 3 grabbed
      - name: Effect
        effect: The target must be the fury's size or smaller. While the target is
          grabbed this way, the fury and their allies gain an edge on strikes
          against them.
  - type: feature
    feature_type: trait
    name: Overpower
    icon: ⭐️
    effects:
      - effect: Once per turn, when the fury force moves a creature or object, or shifts
          adjacent to a creature or object, they can use a signature ability
          against that creature or object.
  - type: feature
    feature_type: trait
    name: Rivalry
    icon: ⭐️
    effects:
      - effect: At the start of an encounter, the fury chooses one creature within their
          line of effect. Both the fury and the creature can add a d3 roll to
          power rolls they make against each other.
~~~