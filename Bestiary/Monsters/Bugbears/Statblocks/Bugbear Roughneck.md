---
agility: 2
ancestry:
- Bugbear
- Fey
- Goblin
- Humanoid
ev: '16'
file_basename: Bugbear Roughneck
file_dpath: Monsters/Bugbears/Statblocks
free_strike: 5
intuition: 0
item_id: bugbear-roughneck
item_index: '289'
item_name: Bugbear Roughneck
level: 2
might: 2
presence: 0
reason: 0
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:bugbear-roughneck
scdc:
- 1.1.1:2:289
size: 1L
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '109'
type: monster
---

~~~ds-statblock
type: statblock
name: Bugbear Roughneck
level: 2
roles:
  - Elite Brute
ancestry:
  - Bugbear
  - Fey
  - Goblin
  - Humanoid
ev: "16"
stamina: "109"
speed: 6
size: 1L
stability: 0
free_strike: 5
might: 2
agility: 2
reason: 0
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Haymaker
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
      - roll: Power Roll + 2
        tier1: 7 damage
        tier2: 11 damage; one target is grabbed; one target is pushed up to 2 squares
        tier3: 14 damage; one target is grabbed; one target is vertical pushed up to 3
          squares
      - cost: 5 Malice
        effect: The ability takes the Area keyword and loses the Strike keyword, its
          distance becomes a 1 burst, and it targets each enemy in the area.
  - type: feature
    feature_type: ability
    name: Leaping Fury
    icon: 🗡
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 8 damage; M < 1 prone
        tier2: 13 damage; M < 2 prone
        tier3: 16 damage; M < 3 prone
      - name: Effect
        effect: The roughneck can jump up to 5 squares to an unoccupied space within
          distance of the target before making this strike.
  - type: feature
    feature_type: ability
    name: Drag Through Hell
    icon: 🗡
    cost: 3 Malice
    keywords:
      - Melee
    usage: Maneuver
    distance: Melee 1
    target: One creature or object
    effects:
      - name: Special
        effect: The target must be grabbed by the roughneck.
      - name: Effect
        effect: The roughneck moves up to their speed across the ground, dragging the
          target with them. The target takes 2 damage for each square they were
          dragged through. When this movement ends, the target is no longer
          grabbed and falls prone. Each square the target was dragged through is
          difficult terrain for enemies.
  - type: feature
    feature_type: ability
    name: Throw
    icon: 🗡
    keywords:
      - Melee
      - Strike
    usage: Maneuver
    distance: Melee 1
    target: One creature or object
    effects:
      - name: Special
        effect: The target must be grabbed by the roughneck.
      - name: Effect
        effect: The target is vertical pushed up to 5 squares. An ally doesn't take
          damage from being force moved this way.
  - type: feature
    feature_type: ability
    name: Catcher
    icon: ❗️
    keywords:
      - Melee
    usage: Free triggered action
    distance: Melee 1
    target: The triggering creature or object
    trigger: A size 1 creature or object is force moved within distance, or a size 1
      ally willingly moves within distance.
    effects:
      - name: Effect
        effect: The target is grabbed by the roughneck.
  - type: feature
    feature_type: ability
    name: Flying Sawblade
    icon: ❗️
    keywords:
      - Melee
    usage: Triggered action
    distance: Self
    target: Self
    trigger: The roughneck is vertical force moved by another creature.
    effects:
      - name: Effect
        effect: The roughneck uses Haymaker against a creature or object at any point
          during the forced movement, or after falling as a result of it.
~~~