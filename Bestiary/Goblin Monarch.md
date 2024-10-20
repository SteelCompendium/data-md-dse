```ds-statblock
name: Goblin Monarch
ancestry:
- Goblin
- Humanoid
roles:
- Boss
level: 1
ev: 24
stamina: 50
immunities: []
weaknesses: []
speed: 6 (climb)
size: 1S
stability: 1
free_strike: 3
might: 2
intuition: 0
agility: 1
reason: -4
presence: -3
traits:
- name: End Effect
  effect: At the end of their turn, the monarch can take 5 damage to end one EoE effect
    affecting them. This damage can’t be reduced in any way.
- name: Crafty
  effect: The monarch doesn’t provoke opportunity attacks by moving.
abilities:
- name: Handaxe
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Ranged
  - Weapon
  distance: Reach 1 or Ranged 5
  target: Two creatures or objects
  t1: 3 damage
  t2: 5 damage
  t3: 7 damage
  effects:
  - name: Effect
    effect: 'An ally within 10 squares of the monarch can make a [[Free Strike|free strike]]. '
- name: Get in Here
  type: Maneuver
  cost: 1 VP
  keywords:
  - Ranged
  distance: Ranged 20
  target: Special
  effects:
  - name: Effect
    effect: 'Two [[Goblin Runner|goblin runners]] appear in unoccupied spaces. '
- name: Meat Shield
  type: Triggered Action
  keywords:
  - Melee
  distance: Reach 1
  target: One ally
  trigger: A creature targets the monarch with an attack.
  effects:
  - name: Effect
    effect: 'The ally becomes the target of the triggering attack instead. '
- name: What Are You Waiting For?
  type: Villain Action 1
  keywords:
  - Area
  distance: 10 burst
  target: Each ally
  effects:
  - name: Effect
    effect: 'Each target can move up to their speed or make a [[Free Strike|free strike]]. '
- name: Focus Fire
  type: Villain Action 2
  keywords:
  - Ranged
  distance: Ranged 10
  target: One enemy
  effects:
  - name: Effect
    effect: 'Each ally within 10 squares of the enemy can move up to their speed toward
      the enemy. '
- name: Kill!
  type: Villain Action 3
  keywords:
  - Area
  distance: 10 burst
  target: Each ally
  effects:
  - name: Effect
    effect: Each target can make a [[Free Strike|free strike]] that deals an extra 1 damage.

```
