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
type: statblock
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
features:
  - type: feature
    feature_type: trait
    name: Solo Monster
    icon: ☠️
    effects:
      - name: End Effect
        effect: At the end of each of their turns, the olothec can take 10 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
      - name: Solo Turns
        effect: The olothec can take two turns each round. They can't take turns
          consecutively.
  - type: feature
    feature_type: trait
    name: Gelatinosis
    icon: ⭐️
    effects:
      - effect: A creature permanently devolves into a slime servant if they spend 1
          continuous minute weakened by Devolving Tentacles, they are reduced to
          0 Stamina by the psychic damage from Devolving Tentacles, or they
          suffer all three transformations from Oozing Transformation.
  - type: feature
    feature_type: ability
    name: Devolving Tentacles
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 3
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        tier1: 11 damage; M < 2 weakened or the target is slimed (save ends)
        tier2: 17 damage; M < 3 weakened or the target is slimed (save ends)
        tier3: 20 damage; M < 4 weakened and the target is slimed (save ends)
      - name: Effect
        effect: A slimed target takes 4 psychic damage whenever they make a power roll.
  - type: feature
    feature_type: ability
    name: Slime Spew
    icon: 🔳
    keywords:
      - Area
      - Weapon
    usage: Main action
    distance: 7 x 2 line within 1
    target: Each creature and object in the area
    effects:
      - roll: Power Roll + 4
        tier1: 6 acid damage; A < 2 push special
        tier2: 10 acid damage; A < 3 push special
        tier3: 13 acid damage; A < 4 push special and prone
      - name: Effect
        effect: Each creature pushed this way is pushed to an unoccupied space in the
          area as far as possible from the olothec.
      - cost: 1 Malice
        effect: The area is difficult terrain. Any creature who enters the area or moves
          within it for the first time on a turn and has A < 3 is knocked prone.
  - type: feature
    feature_type: ability
    name: Oozing Transformation
    icon: 🏹
    cost: 2 Malice
    keywords:
      - Psionic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 10
    target: One creature
    effects:
      - roll: Power Roll + 4
        tier1: 13 psychic damage; I < 2 the target is transformed (save ends)
        tier2: 20 psychic damage; I < 3 the target is transformed (save ends)
        tier3: 23 psychic damage; I < 4 the target is transformed (save ends)
      - name: Effect
        effect: Each time a target is transformed, the Director chooses one of the
          following transformations. When a target ends the transformed effect,
          all transformations on them end.
      - name: Head
        effect: The target's head becomes a ball of slime. They can't communicate and
          have line of effect only within 3 squares.
      - name: Legs
        effect: The target's legs become pillars of ooze. They are slowed while on land
          and can automatically swim at full speed while moving.
      - name: Torso
        effect: The target's arms become gelatinous. They can't benefit from edges or
          double edges and can't gain or use surges.
  - type: feature
    feature_type: ability
    name: Jaunt
    icon: 👤
    keywords:
      - Psionic
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The olothec teleports to an unoccupied space within 10 squares.
          Alternatively, they swap places with a creature or object within 5
          squares of them.
  - type: feature
    feature_type: ability
    name: Liquify
    icon: ❗️
    keywords:
      - Psionic
      - Ranged
    usage: Triggered action
    distance: Ranged 5
    target: Each enemy
    trigger: An enemy within distance deals damage to the olothec.
    effects:
      - name: Effect
        effect: The target takes 8 psychic damage and has psychic weakness 3 until the
          end of the olothec's next turn.
  - type: feature
    feature_type: trait
    name: Primordial Mind
    icon: ⭐️
    effects:
      - effect: The olothec can't be made frightened or taunted.
  - type: feature
    feature_type: trait
    name: Slime Sense
    icon: ⭐️
    effects:
      - effect: A slimed or transformed creature can't have concealment from or be
          hidden from the olothec.
  - type: feature
    feature_type: ability
    name: Horrifying Form
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Psionic
      - Ranged
      - Strike
    usage: "-"
    distance: Ranged 20
    target: Each enemy
    effects:
      - roll: Power Roll + 4
        tier1: 10 psychic damage; P < 2 frightened (save ends)
        tier2: 14 psychic damage; P < 3 frightened (save ends)
        tier3: 17 psychic damage; P < 4 frightened (save ends)
      - name: Effect
        effect: While frightened this way, a target can't make saving throws to end any
          other effects
  - type: feature
    feature_type: ability
    name: Psychic Pulse
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - Area
      - Psionic
    usage: "-"
    distance: 10 burst
    target: Each creature in the area
    effects:
      - name: Effect
        effect: The olothec slides each target up to 5 squares. Each target takes 12
          psychic damage, and if they have M < 3 they are weakened and slimed
          (save ends). A slimed target takes 4 psychic damage whenever they make
          a power roll. Additionally, until the start of their next turn, the
          olothec has damage immunity 4.
  - type: feature
    feature_type: ability
    name: Return to Perfection
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Area
      - Psionic
    usage: "-"
    distance: 10 burst
    target: Each creature in the area
    effects:
      - roll: Power Roll + 4
        tier1: 7 psychic damage; R < 2 the target is devolved (save ends)
        tier2: 13 psychic damage; R < 3 the target is devolved (save ends)
        tier3: 16 psychic damage; R < 3 the target is devolved (save ends)
      - name: Effect
        effect: A devolved creature has a −1 score for all their characteristics other
          than Reason.
~~~