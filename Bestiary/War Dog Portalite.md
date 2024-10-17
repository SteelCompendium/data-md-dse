~~~ds-statblock
name: War Dog Portalite
ancestry:
- Humanoid
- War Dog
roles:
- Ambusher
level: 1
ev: 11
stamina: 20
immunities: []
weaknesses: []
speed: 5 ([[Teleport|teleport]])
size: 1M
stability: 0
free_strike: 3
might: ''
intuition: ''
agility: ''
reason: ''
presence: ''
traits:
- name: Loyalty Collar
  effect: When the portalite dies, they explode, dealing 1d6 damage to each adjacent
    enemy.
abilities:
- name: Corrupted Ash Daggers
  type: Action
  roll: 2d10 + 1
  cost: Signature
  t1: 3 damage; slide 1
  t2: 5 damage; slide 2
  t3: 7 damage; slide 3
  effects:
  - name: '**Keywords**'
    effect: Attack, Melee, Ranged, Weapon
  - name: '**Distance**'
    effect: Reach 1 or Ranged 5
  - name: '**Target**'
    effect: 'One creature or object '
  - name: '**Effect**'
    effect: The power roll gains an edge if any of the portalite’s allies are adjacent
      to the target.
  - name: '**1 VP**'
    effect: 'The portalite [[Teleport|teleports]] the target up to 3 squares before sliding them. '
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
- name: Corrupted Ash [[Teleport]] (Maneuver) ◆ 1 VP
  effects:
  - name: '**Keywords**'
    effect: Magic
  - name: '**Distance**'
    effect: Self
  - name: '**Target**'
    effect: Self
  - name: '**Effect**'
    effect: 'The portalite [[Teleport|teleports]] up to 5 squares and gains an edge on attacks
      this turn. '

~~~