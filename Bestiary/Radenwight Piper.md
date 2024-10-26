```ds-statblock
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
intuition: 2
agility: 0
reason: 0
presence: 1
traits:
- name: Musical Suggestion
  effect: At the end of the piper’s turn, they can choose an adjacent creature and
    slide them 2, ignoring stability.
abilities:
- name: Piercing Trill
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Magic
  - Melee
  - Ranged
  distance: Melee 1 or Ranged 10
  target: One creature or object
  t1: 3 sonic damage; push 1
  t2: 5 sonic damage; push 3
  t3: 7 sonic damage; push 4
  effects:
  - name: Effect
    effect: 'The piper or an ally within distance regains Stamina equal to half the
      damage dealt. '
- name: Vivace Vivace!
  type: Maneuver
  cost: 3 Malice
  keywords:
  - Area
  - Magic
  distance: 5 burst
  target: Each ally in the burst
  effects:
  - name: Effect
    effect: 'Each target who has used their Ready Rodent ability since their last
      turn regains the use of their triggered action. '
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
    effect: 'The piper makes a [[Free Strike|free strike]] against the target. '

```
