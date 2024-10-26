```ds-statblock
name: Kobold Veles
ancestry:
- Humanoid
- Kobold
roles:
- Harrier
- Minion
level: 1
ev: 3
stamina: 5
immunities: []
weaknesses: []
speed: '6'
size: 1S
stability: 0
free_strike: 1
might: 0
intuition: 0
agility: 2
reason: 0
presence: 0
traits:
- name: Shield? Shield!
  effect: The veles has increased Stability by 1 and can act as cover for allies when
    adjacent to an ally who also has this trait.
abilities:
- name: Pilum
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Ranged
  - Weapon
  distance: Melee 1 or Ranged 5
  target: 1 creature or object per minion
  t1: 1 damage
  t2: 2 damage
  effects:
  - name: Effect
    effect: 'All kobolds ignore opportunity attacks from the target until the start
      of the veles’ next turn. '

```
