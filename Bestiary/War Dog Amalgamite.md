~~~ds-statblock
name: War Dog Amalgamite
ancestry:
- Humanoid
- War Dog
roles:
- Brute
level: 2
ev: 15
stamina: 35
immunities: []
weaknesses: []
speed: '5'
size: 1M
stability: 0
free_strike: 4
might: ''
intuition: ''
agility: ''
reason: ''
presence: ''
traits:
- name: Loyalty Collar
  effect: When the amalgamite dies, they explode, dealing 1d6 damage to each adjacent
    enemy.
abilities:
- name: Several Arms
  type: Action
  roll: 2d10 + 2
  cost: Signature
  t1: 4 damage
  t2: 7 damage; [[Grabbed|grabbed]]
  t3: 10 damage; [[Grabbed|grabbed]]
  effects:
  - name: '**Keywords**'
    effect: Attack, Melee, Weapon
  - name: '**Distance**'
    effect: Reach 2
  - name: '**Target**'
    effect: 'One creature or object '
  - name: '**Special**'
    effect: The amalgamite can [[Grab|grab]] up to four creatures.
  - name: '**5 VP**'
    effect: 'The amalgamite deals 4 damage to each creature they have [[Grabbed|grabbed]], and
      regains Stamina equal to the damage dealt. '
- name: Posthumous Promotion
  type: Maneuver
  effects:
  - name: '**Keywords**'
    effect: Magic, Ranged
  - name: '**Distance**'
    effect: Ranged 10
  - name: '**Target**'
    effect: One war dog with a loyalty collar
  - name: '**Effect**'
    effect: 'The target’s loyalty collar detonates, killing them instantly. '

~~~