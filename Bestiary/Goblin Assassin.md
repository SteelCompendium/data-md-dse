```ds-statblock
name: Goblin Assassin
ancestry:
- Goblin
- Humanoid
roles:
- Ambusher
level: 1
ev: 11
stamina: 20
immunities: []
weaknesses: []
speed: 6 (climb)
size: 1S
stability: 0
free_strike: 3
might: -2
intuition: 0
agility: 2
reason: 0
presence: -2
traits:
- name: Crafty
  effect: The assassin doesn't provoke opportunity attacks by moving.
- name: [[Hide]] While Observed
  effect: The assassin can take the [[Hide]] maneuver even while observed, though they
    still must have cover or concealment.
abilities:
- name: Sword
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: One creature or object
  t1: 3 damage
  t2: 5 damage
  t3: 7 damage
  effects:
  - roll: 2d10 + 2
    t1: 3 damage
    t2: 5 damage
    t3: 7 damage
  - name: Effect
    effect: 'This ability has edge if the assassin has an edge on the power roll. '
- name: Shadow Chains
  type: Action
  roll: 2d10 + 2
  cost: 3 Malice
  keywords:
  - Magic
  - Ranged
  distance: Ranged 10
  target: Three creatures
  t1: 3 corruption damage; A1 [[Restrained|restrained]] (save ends)
  t2: 5 corruption damage; A2 [[Restrained|restrained]] (save ends)
  t3: '7 corruption damage; A3 [[Restrained|restrained]] (save ends) '
  effects:
  - roll: 2d10 + 2
    t1: 3 corruption damage; A1 [[Restrained|restrained]] (save ends)
    t2: 5 corruption damage; A2 [[Restrained|restrained]] (save ends)
    t3: '7 corruption damage; A3 [[Restrained|restrained]] (save ends) '

```
