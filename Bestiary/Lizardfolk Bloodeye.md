```ds-statblock
name: Lizardfolk Bloodeye
ancestry:
- Humanoid
- Lizardfolk
roles:
- Hexer
level: 1
ev: 11
stamina: 20
immunities: []
weaknesses: []
speed: 5 (swim)
size: 1M
stability: 0
free_strike: 3
might: 1
intuition: 2
agility: 1
reason: 0
presence: 0
traits:
- name: Reptilian Escape
  effect: While the bloodeye still has a tail, whenever the bloodeye is [[Grabbed|grabbed]], [[Slowed|slowed]],
    [[Weakened|weakened]], or knocked [[Prone|prone]], the bloodeye can lose their tail to immediately end
    the effect and shift 2.
abilities:
- name: Bola Knock
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Ranged
  - Weapon
  distance: Ranged 5
  target: 1 creature or object
  t1: 3 damage
  t2: 5 damage; A1 [[Restrained|restrained]] (save ends)
- name: Bloodshot
  type: Action
  roll: 2d10 + 2
  cost: 2 Malice
  keywords:
  - Attack
  - Ranged
  distance: Ranged 10
  target: 1 creature
  t1: 3 acid damage; M1 target can’t establish line of effect beyond 3 squares (save
    ends)
  t2: 5 acid damage; M2 target can’t establish line of effect beyond 2 squares (save
    ends)

```
