~~~ds-statblock
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
intuition: 1
agility: 1
reason: 0
presence: 0
traits: []
abilities:
- name: Dagger Dance
  type: Action
  roll: 2d10 + 1
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Reach 1 or Ranged 5
  target: One creature per minion
  effect: 'If the mischiever is hidden when they use this ability, they can target
    two creatures. '
- name: Ready Rodent
  type: Triggered Action
  keywords:
  - Melee
  - Weapon
  distance: Reach 1
  target: One creature
  trigger: An ally deals damage to the target.
  effect: The mischiever makes a free strike against the target.

~~~