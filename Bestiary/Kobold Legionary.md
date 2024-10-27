```ds-statblock
name: Kobold Legionary
ancestry:
- Humanoid
- Kobold
roles:
- Defender
level: 1
ev: 9
stamina: 20
immunities: []
weaknesses: []
speed: '5'
size: 1S
stability: 0
free_strike: 1
might: 2
intuition: 0
agility: 1
reason: 0
presence: 0
traits:
- name: Shield? Shield!
  effect: The legionary has increased Stability by 1 and can act as cover for allies
    when adjacent to an ally who also has this trait.
abilities:
- name: Gladius
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: 1 creature or object
  t1: 2 damage
  t2: 4 damage
  effects:
  - name: Effect
    effect: [[Taunted]] (EoT).
  - name: 3 Malice
    effect: 'The legionary and their squad can shift 2 before this attack is made. '
- name: Shield Bash
  type: Maneuver
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: 1 creature or object
  t1: 1 damage; push 1; 1 [[Prone|prone]]
  t2: 2 damage; push 2; 2 [[Prone|prone]]

```
