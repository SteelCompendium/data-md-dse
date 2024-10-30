```ds-statblock
name: [[Dwarf]] Driver
ancestry:
- [[Dwarf]]
- Humanoid
roles:
- Harrier
- Minion
level: 1
ev: 6
stamina: 12
immunities: []
weaknesses: []
speed: '7'
size: 1M
stability: 1
free_strike: 2
might: 2
intuition: 0
agility: 1
reason: 0
presence: 0
traits: []
abilities:
- name: Handaxes
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - [[Charge]]
  - Melee
  - Ranged
  - Weapon
  distance: Melee 1 or Ranged 5
  target: 1 creature or object per minion
  t1: 2 damage; push 1
  t2: 4 damage; push 2
  t3: 5 damage; push 4
  effects:
  - roll: 2d10 + 2
    t1: 2 damage; push 1
    t2: 4 damage; push 2
    t3: 5 damage; push 4
  - name: Effect
    effect: A target [[Restrained|restrained]] by a [[Dwarf|dwarf]] can be pushed by this attack.

```
