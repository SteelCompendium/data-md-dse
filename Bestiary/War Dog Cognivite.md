~~~ds-statblock
name: War Dog Cognivite
ancestry:
- Humanoid
- War Dog
roles:
- Defender
level: 1
ev: 11
stamina: 25
immunities: []
weaknesses: []
speed: 5 ([[Fly|fly]])
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
  effect: When the cognivite dies, they explode, dealing 1d6 damage to each adjacent
    enemy.
abilities:
- name: Synlirii Grafts
  type: Action
  roll: 2d10 + 1
  cost: Signature
  t1: 2 psychic damage; vertical slide 1
  t2: 4 psychic damage; vertical slide 2
  t3: '5 psychic damage; vertical slide 3 '
  effects:
  - name: '**Keywords**'
    effect: Area, Psionic
  - name: '**Distance**'
    effect: 1 burst
  - name: '**Target**'
    effect: 'Each enemy '
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
- name: The Voice (Maneuver) ◆ 1 VP
  effects:
  - name: '**Keywords**'
    effect: Psionic, Ranged
  - name: '**Distance**'
    effect: Ranged 10
  - name: '**Target**'
    effect: Each enemy
  - name: '**Effect**'
    effect: 'The cognivite chooses an ally within 10 squares, then chooses whether
      each target is [[Taunted|taunted]] by the ally (EoT) or has a double bane on attacks against
      the ally (EoT). The same choice must be made for all targets. '

~~~