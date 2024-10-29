```ds-statblock
name: Lizardfolk Tonguer
ancestry:
- Humanoid
- Lizardfolk
roles:
- Artillery
- Minion
level: 1
ev: 6
stamina: 8
immunities: []
weaknesses: []
speed: 5 (swim)
size: 1S
stability: 0
free_strike: 2
might: 0
intuition: 1
agility: 2
reason: 0
presence: 0
traits:
- name: Reptilian Escape
  effect: While the tonguer still has a tail, whenever the tonguer is [[Grabbed|grabbed]], [[Slowed|slowed]],
    [[Weakened|weakened]], or knocked [[Prone|prone]], the tonguer can lose their tail to immediately end
    the effect and shift 2.
abilities:
- name: Tonguelash
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 8
  target: 1 creature or object per minion
  t1: 2 damage; pull 1 or shift 1 towards target
  t2: 5 damage; pull 2 or shift 2 towards target
  t3: 6 damage; pull 3 or shift 3 towards target
  effects:
  - name: Effect
    effect: 'If the target ends up in a space adjacent to the tonguer, they are also
      [[Grabbed|grabbed]]. '

```
