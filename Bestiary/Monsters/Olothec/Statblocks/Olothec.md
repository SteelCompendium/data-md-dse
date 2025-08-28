---
agility: -1
ancestry:
- Horror
- Olothec
ev: '84'
file_basename: Olothec
file_dpath: Monsters/Olothec/Statblocks
free_strike: 7
intuition: 2
item_id: olothec
item_index: '107'
item_name: Olothec
level: 6
might: 4
presence: 3
reason: 4
roles:
- Solo
scc:
- mcdm.monsters.v1:monster:olothec
scdc:
- 1.1.1:2:107
size: '2'
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '450'
type: monster
---

~~~ds-statblock
name: Olothec
level: 6
roles:
  - Solo
ancestry:
  - Horror
  - Olothec
ev: "84"
stamina: "450"
immunities:
  - Psychic 6
speed: 7
movement: Fly, swim
size: "2"
stability: 0
free_strike: 7
might: 4
agility: -1
reason: 4
intuition: 2
presence: 3
traits:
  - name: Solo Monster
    effects:
      - effect: At the end of each of their turns, the olothec can take 10 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
        name: End Effect
      - effect: The olothec can take two turns each round. They can't take turns
          consecutively.
        name: Solo Turns
  - name: Gelatinosis
    effects:
      - effect: A creature permanently devolves into a slime servant if they spend 1
          continuous minute weakened by Devolving Tentacles, they are reduced to
          0 Stamina by the psychic damage from Devolving Tentacles, or they
          suffer all three transformations from Oozing Transformation.
  - name: Primordial Mind
    effects:
      - effect: The olothec can't be made frightened or taunted.
  - name: Slime Sense
    effects:
      - effect: A slimed or transformed creature can't have concealment from or be
          hidden from the olothec.
abilities:
  - name: Devolving Tentacles
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 3
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        t1: 11 damage; M < 2 weakened or the target is slimed (save ends)
        t2: 17 damage; M < 3 weakened or the target is slimed (save ends)
        t3: 20 damage; M < 4 weakened and the target is slimed (save ends)
      - effect: A slimed target takes 4 psychic damage whenever they make a power roll.
        name: Effect
  - name: Slime Spew
    icon: 🔳
    keywords:
      - Area
      - Weapon
    type: Main action
    distance: 7 x 2 line within 1
    target: Each creature and object in the area
    effects:
      - roll: Power Roll + 4
        t1: 6 acid damage; A < 2 push special
        t2: 10 acid damage; A < 3 push special
        t3: 13 acid damage; A < 4 push special and prone
      - effect: Each creature pushed this way is pushed to an unoccupied space in the
          area as far as possible from the olothec.
        name: Effect
      - effect: The area is difficult terrain. Any creature who enters the area or moves
          within it for the first time on a turn and has A < 3 is knocked prone.
        cost: 1 Malice
  - name: Oozing Transformation
    icon: 🏹
    cost: 2 Malice
    keywords:
      - Psionic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 10
    target: One creature
    effects:
      - roll: Power Roll + 4
        t1: 13 psychic damage; I < 2 the target is transformed (save ends)
        t2: 20 psychic damage; I < 3 the target is transformed (save ends)
        t3: 23 psychic damage; I < 4 the target is transformed (save ends)
      - effect: Each time a target is transformed, the Director chooses one of the
          following transformations. When a target ends the transformed effect,
          all transformations on them end.
        name: Effect
      - effect: The target's head becomes a ball of slime. They can't communicate and
          have line of effect only within 3 squares.
        name: Head
      - effect: The target's legs become pillars of ooze. They are slowed while on land
          and can automatically swim at full speed while moving.
        name: Legs
      - effect: The target's arms become gelatinous. They can't benefit from edges or
          double edges and can't gain or use surges.
        name: Torso
  - name: Jaunt
    icon: 👤
    keywords:
      - Psionic
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The olothec teleports to an unoccupied space within 10 squares.
          Alternatively, they swap places with a creature or object within 5
          squares of them.
        name: Effect
  - name: Liquify
    icon: ❗️
    keywords:
      - Psionic
      - Ranged
    type: Triggered action
    distance: Ranged 5
    target: Each enemy
    trigger: An enemy within distance deals damage to the olothec.
    effects:
      - effect: The target takes 8 psychic damage and has psychic weakness 3 until the
          end of the olothec's next turn.
        name: Effect
  - name: Horrifying Form
    icon: ☠️
    cost: Villain Action 1
    keywords:
      - Psionic
      - Ranged
      - Strike
    type: "-"
    distance: Ranged 20
    target: Each enemy
    effects:
      - roll: Power Roll + 4
        t1: 10 psychic damage; P < 2 frightened (save ends)
        t2: 14 psychic damage; P < 3 frightened (save ends)
        t3: 17 psychic damage; P < 4 frightened (save ends)
      - effect: While frightened this way, a target can't make saving throws to end any
          other effects
        name: Effect
  - name: Psychic Pulse
    icon: ☠️
    cost: Villain Action 2
    keywords:
      - Area
      - Psionic
    type: "-"
    distance: 10 burst
    target: Each creature in the area
    effects:
      - effect: The olothec slides each target up to 5 squares. Each target takes 12
          psychic damage, and if they have M < 3 they are weakened and slimed
          (save ends). A slimed target takes 4 psychic damage whenever they make
          a power roll. Additionally, until the start of their next turn, the
          olothec has damage immunity 4.
        name: Effect
  - name: Return to Perfection
    icon: ☠️
    cost: Villain Action 3
    keywords:
      - Area
      - Psionic
    type: "-"
    distance: 10 burst
    target: Each creature in the area
    effects:
      - roll: Power Roll + 4
        t1: 7 psychic damage; R < 2 the target is devolved (save ends)
        t2: 13 psychic damage; R < 3 the target is devolved (save ends)
        t3: 16 psychic damage; R < 3 the target is devolved (save ends)
      - effect: A devolved creature has a −1 score for all their characteristics other
          than Reason.
        name: Effect
~~~