```ds-statblock
name: Lizardfolk Shellguard
ancestry:
- Humanoid
- Lizardfolk
roles:
- Defender
- Minion
level: 1
ev: 7
stamina: 12
immunities: []
weaknesses: []
speed: 5 (swim)
size: 1L
stability: 1
free_strike: 2
might: 2
intuition: ''
agility: 1
reason: 0
presence: 0
traits:
- name: Reptilian Escape
  effect: While the shellguard still has a tail, whenever the shellguard is [[Grabbed|grabbed]],
    [[Slowed|slowed]], [[Weakened|weakened]], or knocked [[Prone|prone]], the shellguard can lose their tail to immediately
    end the effect and shift 2.
abilities:
- name: Shield Smash
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
  t2: 4 damage
  t3: 5 damage
  effects:
  - name: Effect
    effect: 'All allies have **advantage** against the target''s next attack. '

```
