```ds-statblock
name: War Dog Crucibite
ancestry:
- Humanoid
- War Dog
roles:
- Artillery
level: 1
ev: 10
stamina: 15
immunities:
- Psychic 3
weaknesses: []
speed: '5'
size: 1M
stability: 0
free_strike: 2
might: 0
intuition: 0
agility: 1
reason: 0
presence: 0
traits:
- name: Loyalty Collar
  effect: When the crucibite dies, they explode, dealing 1d6 damage to each adjacent
    enemy.
abilities:
- name: Flamebelcher
  type: Action
  roll: 2d10 + 1
  cost: Signature
  keywords:
  - Area
  - Weapon
  distance: 5 × 1 line
  target: Each creature and object
  t1: 2 fire damage
  t2: 5 fire damage
  t3: 6 fire damage
  effects:
  - name: Effect
    effect: The area is covered in sticky fire until the start of the crucibite’s
      next turn. Whenever a creature enters the area for the first time in a round
      or starts their turn there, they take 2 fire damage.
  - name: '**2 VP**'
    effect: 'The area increases to a 10 × 1 line, and if any ally of the crucibite
      is in the area when it is created, the crucibite gains an edge on the power
      roll. '
- name: Posthumous Promotion
  type: Maneuver
  keywords:
  - Magic
  - Ranged
  distance: Ranged 10
  target: One war dog with a loyalty collar
  effects:
  - name: Effect
    effect: 'The target’s loyalty collar detonates, killing them instantly. '

```
