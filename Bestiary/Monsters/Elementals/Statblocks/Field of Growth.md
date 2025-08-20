---
agility: 0
ancestry:
- Elemental
ev: '28'
file_basename: Field of Growth
file_dpath: Monsters/Elementals/Statblocks
free_strike: 6
intuition: 2
item_id: field-of-growth
item_index: '324'
item_name: Field of Growth
level: 3
might: 2
presence: 2
reason: 0
roles:
- Elite Controller
scc:
- mcdm.monsters.v1:monster:field-of-growth
scdc:
- 1.1.1:2:324
size: '3'
source: mcdm.monsters.v1
speed: 8
stability: 2
stamina: '120'
type: monster
---

```ds-statblock
name: Field of Growth
level: 3
roles:
  - Elite Controller
ancestry:
  - Elemental
ev: "28"
stamina: "120"
immunities:
  - Poison 5
speed: 8
movement: Climb
size: "3"
stability: 2
free_strike: 6
might: 2
agility: 0
reason: 0
intuition: 2
presence: 2
traits:
  - name: Fickle and Free
    effects:
      - effect: The field can't be restrained, slowed, or knocked prone, and they ignore
          difficult terrain.
  - name: Roots Run Deep
    effects:
      - effect: The field can target any creature touching the ground with their
          abilities, even if they don't have line of effect to that creature.
abilities:
  - name: Hampering Roots
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 8
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        t1: 8 damage
        t2: 13 damage; R < 1 prone and can't stand (save ends)
        t3: 16 damage; R < 2 prone and can't stand (save ends)
      - effect: If a target made prone this way is already prone, they are instead
          restrained (save ends). If the target was also unable to stand, that
          effect ends when they are no longer restrained this way.
  - name: Convocation of Verdure
    keywords:
      - Magic
      - Ranged
    type: Maneuver
    distance: Ranged 5
    target: Self or one elemental
    effects:
      - effect: The target gains 15 temporary Stamina that lasts until the start of the
          field's next turn.
      - effect: Until the end of the encounter, the ground within 1 square of the target
          is overgrown with underbrush and vines. Whenever any enemy makes a
          strike against the target while within line of effect of that area,
          the enemy is pulled 5 squares toward the area after the strike is
          resolved. Any enemy who enters the area for the first time in a round
          or starts their turn there is knocked prone.
        cost: 3 Malice
  - name: Rose Thorn Lash
    cost: 1 Malice
    keywords:
      - Magic
      - Melee
    type: Triggered action
    distance: Melee 3
    target: The triggering creature or object
    trigger: A creature or object within distance deals damage to the field.
    effects:
      - effect: The target takes 6 damage, and if they have A < 2, they are bleeding
          (save ends).
```