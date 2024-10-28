```ds-statblock
name: Kobold Tiro
ancestry:
- Humanoid
- Kobold
roles:
- Defender
- Minion
level: 1
ev: 3
stamina: 8
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
  effect: The tiro has increased Stability by 1 and can act as cover for allies when
    adjacent to an ally who also has this trait.
abilities:
- name: Pugio
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 2
  target: 1 creature or object per minion
  t1: 1 damage
  t2: 2 damage; shift 1
  t3: '3 damage; shift 2 '

```
