~~~ds-statblock
name: War Dog Phosphorite
ancestry:
- Humanoid
- War Dog
roles:
- Hexer
level: 2
ev: 10
stamina: 20
immunities:
- Acid 3
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
  effect: When the phosphorite dies, they explode, dealing 1d6 damage to each adjacent
    enemy.
abilities:
- name: Caustic Detonator (Action) ◆ MGT RR ◆ Signature
  t3: 7 acid damage; [[Bleeding|bleeding]] (MGT ends)
  t2: 5 acid damage; [[Bleeding|bleeding]] (EoT)
  t1: 3 acid damage
  effects:
  - name: '**Keywords**'
    effect: Magic, Ranged, Resistance
  - name: '**Distance**'
    effect: Ranged 10
  - name: '**Target**'
    effect: One creature or object
  - name: '**Effect**'
    effect: 'A detonator attaches to the target. At the end of each round, roll a
      die. On an odd result, the detonator explodes, triggering the resistance roll. '
  - name: '**Special**'
    effect: 'An adjacent creature can attempt an easy Agility test to remove the detonator
      as a maneuver. A failure does nothing, a success disarms and destroys the detonator,
      and a success with a reward allows the disarming creature to throw the detonator
      onto another target within 5 squares. '
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