```ds-statblock
name: [[Dwarf]] Gunner
ancestry:
- [[Dwarf]]
- Humanoid
roles:
- Artillery
level: 1
ev: 12
stamina: 26
immunities: []
weaknesses: []
speed: '5'
size: 1M
stability: 1
free_strike: 3
might: 0
intuition: 1
agility: 2
reason: 0
presence: 0
traits:
- name: Split Shot
  effect: Whenever the gunner deals damage to a creature or object, a creature or
    object within 1 of the recipient takes 3 damage.
abilities:
- name: Portable Ballista
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Ranged
  - Weapon
  distance: Ranged 10
  target: 1 creature or object
  t1: 4 damage; push 1
  t2: 7 damage; push 3
  t3: 10 damage; push 5
  effects:
  - name: Effect
    effect: If the target is adjacent to a wall or object after the power roll is
      resolved, they are [[Restrained|restrained]] (EoT). A target [[Restrained|restrained]] by a [[Dwarf|dwarf]] can be pushed
      by this attack.
  - name: 5 Malice
    effect: 'If the target is pushed into another creature, both the target and the
      creature are [[Restrained|restrained]] (EoT). '
- name: Ensnaring Chains
  type: Maneuver
  cost: 5 Malice
  keywords:
  - Ranged
  - Weapon
  distance: Ranged 10
  target: 1 [[Restrained|restrained]], [[Slowed|slowed]], or [[Prone|prone]] target
  effects:
  - name: Effect
    effect: 'The gunner makes a [[Free Strike|free strike]] against the target. The target loses any
      [[Restrained|restrained]], [[Slowed|slowed]], or [[Prone|prone]] conditions and gains [[Restrained|restrained]] (save ends). '

```
