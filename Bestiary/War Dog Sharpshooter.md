~~~ds-statblock
name: War Dog Sharpshooter
ancestry:
- Humanoid
- War Dog
roles:
- Artillery
- Minion
level: 1
ev: 4
stamina: 8
immunities: []
weaknesses: []
speed: '7'
size: 1M
stability: 0
free_strike: 2
might: ''
intuition: ''
agility: ''
reason: ''
presence: ''
traits:
- name: Loyalty Collar
  effect: When the sharpshooter dies, they explode, dealing 1d6 damage to each adjacent
    enemy.
abilities:
- name: Bolt Launcher
  type: Action
  roll: 2d10 + 1
  cost: Signature
  t1: 2 damage
  t2: 3 damage
  t3: 4 damage
  effects:
  - name: '**Keywords**'
    effect: Attack, Ranged, Weapon
  - name: '**Distance**'
    effect: Ranged 5
  - name: '**Target**'
    effect: 'One creature or object per minion '
  - name: '**Effect**'
    effect: 'This ability ignores cover and concealment. '

~~~