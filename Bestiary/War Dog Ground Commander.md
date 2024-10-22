```ds-statblock
name: War Dog Ground Commander
ancestry:
- Humanoid
- War Dog
roles:
- Boss
level: 3
ev: 36
stamina: 90
immunities: []
weaknesses: []
speed: '5'
size: 1M
stability: 2
free_strike: 5
might: 2
intuition: 2
agility: 2
reason: 2
presence: 2
traits:
- name: End Effect
  effect: At the end of their turn, the ground commander can take 5 damage to end
    one EoE effect affecting them. This damage can’t be reduced in any way.
- name: Loyalty Collar
  effect: When the ground commander dies, they explode, dealing 2d6 damage to each
    adjacent enemy.
abilities:
- name: Conditioning Spear (Action) ◆ 2d10 + 2 ◆ Signature
  keywords:
  - Attack
  - Melee
  - Ranged
  - Weapon
  distance: Reach 1 or Ranged 5
  target: Two creatures or objects
  t1: 5 damage; pull 1
  t2: 8 damage; pull 2
  t3: 11 damage; pull 3
  effects:
  - name: Effect
    effect: One ally within 10 squares of the commander can make a [[Free Strike|free strike]].
  - name: '**1 VP**'
    effect: 'A target who is adjacent to the ground commander after this ability is
      resolved is [[Grabbed|grabbed]] (INU ends). This [[Grab|grab]] can’t be escaped using the Escape
      [[Grab]] maneuver. The ground commander can [[Grab|grab]] up to two creatures at a time. '
- name: Highest Posthumous Promotion
  type: Maneuver
  keywords:
  - Area
  - Magic
  distance: 10 burst
  target: Each war dog with a loyalty collar
  effects:
  - name: Effect
    effect: 'The target’s loyalty collar detonates, killing them instantly. '
- name: Final Orders
  type: [[Triggered Action]]
  keywords:
  - Magic
  - Ranged
  distance: Ranged 10
  target: One ally
  effects:
  - name: '**Trigger**'
    effect: The target has a condition imposed on them, is force moved, or is killed.
  - name: Effect
    effect: 'The target can move up to their speed and make a [[Free Strike|free strike]] before the
      triggering effect happens. '
- name: Combined Arms
  type: Villain Action 1
  keywords:
  - Area
  distance: 10 burst
  target: Each ally
  effects:
  - name: Effect
    effect: 'Each target can make a ranged [[Free Strike|free strike]], then immediately use the [[Charge]]
      action. '
- name: Make an Example of Them
  type: Villain Action 2
  keywords:
  - Magic
  - Ranged
  distance: Ranged 10
  target: One enemy
  effects:
  - name: Effect
    effect: 'Each ally within 5 squares of the target can move up to their speed and
      make a [[Free Strike|free strike]] against the target. The target is then [[Frightened|frightened]] of the
      ground commander (INU ends). '
- name: Claim Them for the Body Banks
  type: Villain Action 3
  keywords:
  - Area
  - Magic
  distance: 10 burst
  target: Each ally
  effects:
  - name: Effect
    effect: Each target can shift up to 2 squares and use the [[Grab]] maneuver. For the
      rest of the encounter, any enemy takes a bane on the [[Escape Grab]] maneuver.

```
