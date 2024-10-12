~~~ds-statblock
name: Radenwight Piper
ancestry:
- Humanoid
- Radenwight
roles:
- Support
level: 1
ev: 13
stamina: 30
immunities: []
weaknesses: []
speed: 5 (climb)
size: 1S
stability: 0
free_strike: 2
might: 0
intuition: 1
agility: 0
reason: 0
presence: 1
traits: []
abilities:
- name: Piercing Trill
  type: Action
  roll: 2d10 + 1
  cost: Signature
  keywords:
  - Attack
  - Magic
  - Melee
  - Ranged
  distance: Reach 1 or Ranged 10
  target: One creature or object
  effect: 'The piper or an ally within distance regains stamina equal to half the
    damage dealt. '
- name: Vivace Vivace!
  type: Maneuver
  keywords:
  - Area
  - Magic
  distance: 5 burst
  target: Each ally
  effect: 'Each target who has used their Ready Rodent ability since their last turn
    regains the use of their triggered action. '
- name: Ready Rodent
  type: Triggered Action
  keywords:
  - Melee
  - Weapon
  distance: Reach 1
  target: One creature
  trigger: An ally deals damage to the target.
  effect: The piper makes a free strike against the target.

~~~