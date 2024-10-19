```ds-statblock
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
might: 2
intuition: 0
agility: 0
reason: 0
presence: 0
traits:
- name: Loyalty Collar
  effect: When the amalgamite dies, they explode, dealing 1d6 damage to each adjacent
    enemy.
abilities:
- name: Several Arms
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Reach 2
  target: One creature or object
  t1: 4 damage
  t2: 7 damage; [[Grabbed|grabbed]]
  t3: 10 damage; [[Grabbed|grabbed]]
  effects:
  - name: '**Special**'
    effect: The amalgamite can [[Grab|grab]] up to four creatures.
  - name: '**5 VP**'
    effect: 'The amalgamite deals 4 damage to each creature they have [[Grabbed|grabbed]], and
      regains Stamina equal to the damage dealt. '
- name: Posthumous Promotion
  type: Maneuver
  keywords:
  - Magic
  - Ranged
  distance: Ranged 10
  target: One war dog with a loyalty collar
  effects:
  - name: Effect
    effect: 'The target’s loyalty collar detonates, killing them instantly. '

```
