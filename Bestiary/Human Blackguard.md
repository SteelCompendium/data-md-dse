```ds-statblock
name: [[Human]] Blackguard
ancestry:
- [[Human]]
- Humanoid
roles:
- Boss
level: 1
ev: 38
stamina: 80
immunities:
- Magic 2
- Psionic 2
weaknesses: []
speed: '5'
size: 1M
stability: 2
free_strike: 4
might: 2
intuition: 0
agility: 2
reason: 2
presence: 2
traits:
- name: End Effect
  effect: At the end of their turn, the blackguard can take 5 damage to end one EoE
    effect affecting them. This damage can’t be reduced in any way.
abilities:
- name: Zweihander
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Reach 1
  target: Each adjacent enemy
  t1: 4 damage
  t2: 7 damage; [[Slowed|slowed]] (EoT)
  t3: 10 damage; [[Slowed|slowed]] (MGT ends)
  effects:
  - name: Effect
    effect: An ally within 10 squares of the blackguard can make a [[Free Strike|free strike]].
- name: You!
  type: Maneuver
  keywords:
  - Ranged
  distance: Ranged 10
  target: One enemy
  effects:
  - name: Effect
    effect: 'The target is marked until the start of the blackguard’s next turn. The
      blackguard and each of their allies gain an edge on attacks against any target
      marked by the blackguard, and such attacks deal an extra 2 damage. '
- name: [[Parry]]!
  type: Triggered Action
  keywords:
  - Melee
  - Weapon
  distance: Reach 1
  target: Self or one ally
  trigger: A creature targets the blackguard or an ally adjacent to the blackguard
    with an attack.
  effects:
  - name: Effect
    effect: 'The triggering attack’s damage is halved. '
- name: Advance!
  type: Villain Action 1
  keywords:
  - Weapon
  distance: Self
  target: Self
  effects:
  - name: Effect
    effect: 'The blackguard shifts up to their speed. During or after this movement,
      they can make two Zweihander attacks. '
- name: Back!
  type: Villain Action 2
  keywords:
  - Area
  - Magic
  distance: 5 burst
  target: Each enemy
  effects:
  - name: Effect
    effect: 'The blackguard slides each target 5 squares. '
- name: I Can Throw My Blade and So Should You!
  type: Villain Action 3
  keywords:
  - Area
  - Magic
  - Ranged
  - Weapon
  distance: 3 cube within 5
  target: Each enemy in the cube
  effects:
  - name: Effect
    effect: The blackguard makes a Zweihander attack against each enemy in the area,
      making one power roll against all targets. Additionally, each ally within 5
      squares of the area can make a [[Free Strike|free strike]] against any enemy in the area.

```
