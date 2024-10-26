```ds-statblock
name: Radenwight Mischiever
ancestry:
- Humanoid
- Radenwight
roles:
- Ambusher
- Minion
level: 1
ev: 7
stamina: 10
immunities: []
weaknesses: []
speed: 7 (climb)
size: 1S
stability: 0
free_strike: 2
might: -1
intuition: 0
agility: 2
reason: 0
presence: 0
traits: []
abilities:
- name: Dagger Dance
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1 or Ranged 5
  target: One creature per minion
  t1: 2 damage
  t2: 5 damage
  t3: 6 damage
  effects:
  - name: Effect
    effect: 'If the mischief is hidden when they use this ability, they can target
      two creatures. '
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
    effect: The mischief makes a [[Free Strike|free strike]] against the target.

```
