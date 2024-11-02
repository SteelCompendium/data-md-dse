```ds-statblock
name: Radenwight Redeye
ancestry:
- Humanoid
- Radenwight
roles:
- Artillery
- Minion
level: 1
ev: 6
stamina: 8
immunities: []
weaknesses: []
speed: 5 (climb)
size: 1S
stability: 0
free_strike: 2
might: 1
intuition: 0
agility: 2
reason: -1
presence: 0
traits: []
abilities:
- name: Eyes-On-Me Shot
  type: Action
  cost: Signature
  keywords:
  - Attack
  - Ranged
  - Weapon
  distance: Ranged 10
  target: One creature or object per minion
  effects:
  - roll: 2d10 + 2
    t1: 2 damage
    t2: 5 damage
    t3: 6 damage
  - name: Effect
    effect: 'An ally of the redeye within 2 squares of the target can shift up to
      2 squares. '
- name: Ready Rodent
  type: Triggered Action
  keywords:
  - Melee
  - Weapon
  distance: Melee 1
  target: One creature
  trigger: An ally deals damage to the target.
  effects:
  - name: Effect
    effect: The redeye makes a [[Free Strike|free strike]] against the target.

```
