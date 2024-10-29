```ds-statblock
name: Lizardfolk Grunt
ancestry:
- Humanoid
- Lizardfolk
roles:
- Harrier
- Minion
level: 1
ev: 6
stamina: 10
immunities: []
weaknesses: []
speed: 6 (swim)
size: 1M
stability: 0
free_strike: 2
might: 1
intuition: 0
agility: 2
reason: 0
presence: 0
traits:
- name: Reptilian Escape
  effect: While the grunt still has a tail, whenever the grunt is [[Grabbed|grabbed]], [[Slowed|slowed]],
    [[Weakened|weakened]], or knocked [[Prone|prone]], the grunt can lose their tail to immediately end the
    effect and shift 2.
abilities:
- name: Snap and Toss
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: 1 creature or object per minion
  t1: 2 damage
  t2: 4 damage; slide 2
  t3: '5 damage; slide 4 '

```
