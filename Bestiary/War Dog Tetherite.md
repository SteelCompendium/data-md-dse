```ds-statblock
name: War Dog Tetherite
ancestry:
- Humanoid
- War Dog
roles:
- Brute
- Minion
level: 1
ev: 6
stamina: 8
immunities: []
weaknesses: []
speed: '5'
size: 1M
stability: 0
free_strike: 2
might: 2
intuition: 0
agility: 0
reason: 0
presence: 0
traits:
- name: Tethered
  effect: A captain attached to a tetherite squad has their Stability increased by
    the number of tetherites within 2 squares of them.
- name: Loyalty Collar
  effect: When the tetherite dies, they explode, dealing 1d6 damage to each adjacent
    enemy.
abilities:
- name: Banded Dagger
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 2
  target: One creature or object per minion
  t1: 2 damage
  t2: 4 damage
  t3: '5 damage '

```
