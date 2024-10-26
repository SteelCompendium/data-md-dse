```ds-statblock
name: [[Dwarf]] Hunter
ancestry:
- [[Dwarf]]
- Humanoid
roles:
- Support
- Minion
level: 1
ev: 6
stamina: 12
immunities: []
weaknesses: []
speed: '5'
size: 1M
stability: 1
free_strike: 2
might: 1
intuition: 0
agility: 2
reason: 0
presence: 0
traits: []
abilities:
- name: Snaring Javelin
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Ranged
  - Weapon
  distance: Ranged 5
  target: 1 creature or object per minion
  t1: 2 damage; pull 1
  t2: 4 damage; pull 2
  effects:
  - name: '**Effect**'
    effect: A target [[Restrained|restrained]] by a [[Dwarf|dwarf]] can be pulled by this attack.

```
