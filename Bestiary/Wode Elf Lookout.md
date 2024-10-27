```ds-statblock
name: Wode Elf Lookout
ancestry:
- Fey
- Humanoid
- Wode Elf
roles:
- Support
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
- name: There!
  effect: A wode elf within 5 of the lookout can make a ranged attack as if occupying
    the lookout's space.
- name: Masking Glamor
  effect: The lookout immediately [[Hide|hides]] at the end of their turn while in cover or
    concealment, even if they are observed.
abilities:
- name: Longbow
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Ranged
  - Weapon
  distance: Ranged 8
  target: 1 creature or object per minion
  t1: 2 damage
  t2: 4 damage
  t3: '5 damage '

```
