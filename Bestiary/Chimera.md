```ds-statblock
name: Chimera
ancestry:
- Monster
roles:
- SOLO
level: 3
ev: 88
stamina: 240
immunities:
- Fire 6
weaknesses: []
speed: 10 ([[Fly|fly]])
size: '2'
stability: 1
free_strike: 6
might: 3
intuition: 1
agility: 2
reason: -2
presence: 0
traits:
- name: Solo Monster
  effect: '- **Solo Turns:** The chimera takes 2 turns each round. They can use two
    actions on each of their turns and can take each turn after an enemy turn they
    choose. While [[Dazed|dazed]], the chimera can take one action and one maneuver per turn.  **End
    Effect:** At the end of their turn, the chimera can take 5 damage to end one save
    ends effect affecting them. This damage can''t be reduced in any way.'
- name: Volant
  effect: When the chimera makes a creature winded or reduces them to 0 Stamina or
    less, the chimera can move their speed towards one enemy within line of effect.
abilities:
- name: Bite
  type: Action
  roll: 2d10 + 3
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 2
  target: 2 creatures or objects
  t1: 6 damage
  t2: 10 damage
  t3: 13 damage
  effects:
  - roll: 2d10 + 3
    t1: 6 damage
    t2: 10 damage
    t3: 13 damage
  - name: Effect
    effect: 'This attack has an edge if the chimera has an edge on the attack. '
- name: Dragon's Eruption
  type: Action
  roll: AGL RR
  cost: 7 Malice
  keywords:
  - Area
  - Magic
  distance: 3 cube within 10
  target: All enemies in the cube
  t1: 13 fire damage
  t2: 10 fire damage
  t3: '6 fire damage '
  effects:
  - roll: AGL RR
    t1: 13 fire damage
    t2: 10 fire damage
    t3: '6 fire damage '
- name: Lion's Toss
  type: Maneuver
  roll: 2d10 + 3
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 2
  target: 1 creature or object
  t1: vertical push 1
  t2: vertical push 3
  t3: 'vertical push 5 '
  effects:
  - roll: 2d10 + 3
    t1: vertical push 1
    t2: vertical push 3
    t3: 'vertical push 5 '
- name: Roar
  type: Action
  roll: 2d10 + 3
  cost: 5 Malice
  keywords:
  - Area
  - Magic
  distance: 5 burst
  target: All enemies in the burst
  t1: 4 psychic damage
  t2: 8 psychic damage; I2 [[Frightened|frightened]] (save ends)
  t3: '10 psychic damage; I3 [[Frightened|frightened]] (save ends) '
  effects:
  - roll: 2d10 + 3
    t1: 4 psychic damage
    t2: 8 psychic damage; I2 [[Frightened|frightened]] (save ends)
    t3: '10 psychic damage; I3 [[Frightened|frightened]] (save ends) '
- name: Ram's Defiance
  type: Triggered Action
  roll: 2d10 + 3
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Ranged 5
  target: 1 creature
  trigger: The target attacks the chimera and gets a tier-1 result.
  t1: 3 damage; M2 [[Slowed|slowed]] (save ends)
  t2: 5 damage; [[Prone|prone]]; M3 [[Slowed|slowed]] (save ends)
  t3: '7 damage; [[Prone|prone]]; M4 [[Slowed|slowed]] (save ends) '
  effects:
  - roll: 2d10 + 3
    t1: 3 damage; M2 [[Slowed|slowed]] (save ends)
    t2: 5 damage; [[Prone|prone]]; M3 [[Slowed|slowed]] (save ends)
    t3: '7 damage; [[Prone|prone]]; M4 [[Slowed|slowed]] (save ends) '
  - name: Effect
    effect: The chimera shifts 5. If they end this movement adjacent to the target,
      roll power.
- name: Overture of Destruction
  type: Villain Action 1
  keywords:
  - Area
  - Melee
  - Weapon
  distance: 1 burst
  target: All enemies in the burst
  effects:
  - name: Effect
    effect: 'The chimera uses Bite and Lion''s Toss against each target. '
- name: Fire Solo
  type: Villain Action 2
  keywords:
  - Area
  - Melee
  - Weapon
  distance: Self
  target: Self
  effects:
  - name: Effect
    effect: 'The chimera uses Dragon''s Eruption and Roar without spending malice. '
- name: Chorus of Destruction
  type: Villain Action 3
  keywords:
  - '-'
  distance: Self
  target: Self
  effects:
  - name: Effect
    effect: The chimera uses Roar. The chimera then shifts their speed and can make
      a [[Free Strike|free strike]] against each enemy who comes within 1 of them during the move.
      When the chimera ends this movement, they use Dragon's Eruption.

```
