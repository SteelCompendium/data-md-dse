```ds-statblock
name: [[Human]] Trickshot
ancestry:
- [[Human]]
- Humanoid
roles:
- Artillery
level: 1
ev: 12
stamina: 20
immunities:
- Magic 2
- Psionic 2
weaknesses: []
speed: '5'
size: 1M
stability: 0
free_strike: 4
might: 0
intuition: 0
agility: 1
reason: 0
presence: 0
traits: []
abilities:
- name: Crossbow
  type: Action
  roll: 2d10 + 1
  cost: Signature
  keywords:
  - Attack
  - Ranged
  - Weapon
  distance: Ranged 15
  target: One creature or object
  t1: 4 damage
  t2: 7 damage
  t3: 10 damage
  effects:
  - name: Effect
    effect: The trickshot doesn’t take a bane when using this ability in melee or
      against a target with cover or concealment.

```
