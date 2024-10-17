~~~ds-statblock
name: War Dog Pestilite
ancestry:
- Humanoid
- War Dog
roles:
- Controller
level: 3
ev: 13
stamina: 25
immunities:
- Poison 3
weaknesses: []
speed: '5'
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
  effect: When the pestilite dies, they explode, dealing 1d6 damage to each adjacent
    enemy.
abilities:
- name: Plaguecaster (Action) ◆ INU RR ◆ Signature
  t3: 8 poison damage; [[Frightened|frightened]] (INU ends)
  t2: 5 poison damage; [[Frightened|frightened]] (EoT)
  t1: 2 poison damage
  effects:
  - name: '**Keywords**'
    effect: Area, Magic, Ranged, Resistance
  - name: '**Distance**'
    effect: 3 cube within 10
  - name: '**Target**'
    effect: 'Each creature '
  - name: '**Effect**'
    effect: 'The area is covered in a cloud of pestilence that lasts until the start
      of the pestilite’s next turn. Any creature who enters the area for the first
      time in a round or starts their turn there takes 2 poison damage. '
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