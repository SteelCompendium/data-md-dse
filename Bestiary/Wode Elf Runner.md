```ds-statblock
name: Wode Elf Runner
ancestry:
- Fey
- Humanoid
- Wode Elf
roles:
- Harrier
- Minion
level: 1
ev: ''
stamina: ''
immunities: []
weaknesses: []
speed: ''
size: ''
stability: ''
free_strike: ''
might: 0
intuition: 0
agility: 2
reason: 0
presence: 1
traits:
- name: Masking Glamor
  effect: The runner immediately [[Hide|hides]] at the end of their turn while in cover or
    concealment, even if they are observed.
abilities:
- name: Spear
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
  t1: 2 damage
  t2: 4 damage
  t3: 5 damage
  effects:
  - name: Effect
    effect: 'The runner can shift 2 before making the attack. '

```
