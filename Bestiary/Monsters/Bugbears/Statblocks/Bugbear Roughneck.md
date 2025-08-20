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
item_index: '291'
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
- 1.1.1:2:291
size: 1L
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '109'
type: monster
---

```ds-statblock
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
traits: []
abilities:
  - name: Haymaker
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        t1: 7 damage
        t2: 11 damage; one target is grabbed; one target is pushed up to 2 squares
        t3: 14 damage; one target is grabbed; one target is vertical pushed up to 3
          squares
      - effect: The ability takes the Area keyword and loses the Strike keyword, its
          distance becomes a 1 burst, and it targets each enemy in the area.
        cost: 5 Malice
  - name: Leaping Fury
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 8 damage; M < 1 prone
        t2: 13 damage; M < 2 prone
        t3: 16 damage; M < 3 prone
      - effect: The roughneck can jump up to 5 squares to an unoccupied space within
          distance of the target before making this strike.
  - name: Drag Through Hell
    cost: 3 Malice
    keywords:
      - Melee
    type: Maneuver
    distance: Melee 1
    target: One creature or object
    effects:
      - effect: The target must be grabbed by the roughneck.
        name: Special
      - effect: The roughneck moves up to their speed across the ground, dragging the
          target with them. The target takes 2 damage for each square they were
          dragged through. When this movement ends, the target is no longer
          grabbed and falls prone. Each square the target was dragged through is
          difficult terrain for enemies.
  - name: Throw
    keywords:
      - Melee
      - Strike
    type: Maneuver
    distance: Melee 1
    target: One creature or object
    effects:
      - effect: The target must be grabbed by the roughneck.
        name: Special
      - effect: The target is vertical pushed up to 5 squares. An ally doesn't take
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
      - effect: The target is grabbed by the roughneck.
  - name: Flying Sawblade
    keywords:
      - Melee
    type: Triggered action
    distance: Self
    target: Self
    trigger: The roughneck is vertical force moved by another creature.
    effects:
      - effect: The roughneck uses Haymaker against a creature or object at any point
          during the forced movement, or after falling as a result of it.
```