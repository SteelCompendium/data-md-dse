```ds-statblock
name: [[Human]] Bandit Chief
ancestry:
- [[Human]]
- Humanoid
roles:
- Boss
level: 3
ev: 54
stamina: 120
immunities:
- Magic 2
- Psionic 2
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
  effect: At the end of their turn, the bandit chief can take 5 damage to end one
    EoE effect affecting them. This damage can’t be reduced in any way.
abilities:
- name: Whip & Magic Longsword
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Magic
  - Melee
  - Weapon
  distance: Reach 1
  target: Two enemies or objects
  t1: 5 damage; pull 1
  t2: 9 damage; pull 2
  t3: 12 damage; pull 3
  effects:
  - name: Effect
    effect: A target who is adjacent to the bandit chief after the attack is resolved
      takes 9 corruption damage.
- name: Kneel, Peasant!
  type: Maneuver
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Reach 1
  target: One enemy or object
  t1: Push 1
  t2: Push 2; [[Prone|prone]]
  t3: Push 3; [[Prone|prone]]
- name: Bloodstones
  type: Triggered Action
  keywords:
  - Magic
  distance: Self
  target: Self
  trigger: The bandit chief makes a power roll for an attack.
  effects:
  - name: Effect
    effect: 'The bandit chief takes 4 corruption damage and increases the result of
      the power roll by one tier. '
- name: Shoot!
  type: Villain Action 1
  keywords:
  - Area
  distance: 10 burst
  target: Each ally
  effects:
  - name: Effect
    effect: 'Each target can make a ranged [[Free Strike|free strike]]. '
- name: Form Up!
  type: Villain Action 2
  keywords:
  - Area
  distance: 10 burst
  target: Each ally
  effects:
  - name: Effect
    effect: 'Each target shifts up to their speed. Until the end of the encounter,
      any enemy takes a bane on attacks against the bandit chief or any of the bandit
      chief’s allies if they are adjacent to that target. '
- name: Lead From the Front
  type: Villain Action 3
  keywords:
  - Attack
  - Weapon
  distance: Self
  target: Self
  effects:
  - name: Effect
    effect: The bandit chief shifts twice their speed. During or after this movement,
      they can attack up to four targets with Whip & Magic Longsword. Any ally of
      the bandit chief adjacent to a target can make a [[Free Strike|free strike]] against that target.

```
