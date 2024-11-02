```ds-statblock
name: Kobold Sagittarius
ancestry:
- Humanoid
- Kobold
roles:
- Artillery
- Minion
level: 1
ev: 2
stamina: 4
immunities: []
weaknesses: []
speed: '5'
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
  effect: The sagittarius has increased Stability by 1 and can act as cover for allies
    when adjacent to an ally who also has this trait.
abilities:
- name: Composite Bow
  type: Action
  cost: Signature
  keywords:
  - Attack
  - Ranged
  - Weapon
  distance: Ranged 10
  target: 1 creature or object per minion
  effects:
  - roll: 2d10 + 2
    t1: 2 damage
    t2: 3 damage
    t3: 4 damage
  - name: Effect
    effect: 'The sagittarius has increased Stability while adjacent to an ally. '

```
