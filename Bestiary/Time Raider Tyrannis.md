```ds-statblock
name: [[Time Raider]] Tyrannis
ancestry:
- Humanoid
- [[Time Raider]]
roles:
- Boss
level: 3
ev: 54
stamina: 120
immunities:
- Psychic 7
weaknesses: []
speed: 10 ([[Fly|fly]], [[Teleport|teleport]])
size: '2'
stability: 0
free_strike: 5
might: 0
intuition: 1
agility: 3
reason: 3
presence: 0
traits:
- name: End Effect
  effect: At the end of their turn, the tyrannis can take 5 damage to end one EoE
    effect affecting them. This damage can’t be reduced in any way.
- name: Foresight
  effect: The tyrannis doesn’t take a bane on attacks against concealed creatures.
abilities:
- name: Gatling Blaster
  type: Action
  roll: 2d10 + 3
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Ranged
  - Psionic
  - Weapon
  distance: Reach 2 or Ranged 10
  target: Three creatures or objects
  t1: 5 corruption damage
  t2: 9 corruption damage
  t3: 12 corruption damage
  effects:
  - name: Effect
    effect: 'Each target’s speed is reduced by 2 (EoT). '
- name: Air Raid!
  type: Maneuver
  cost: 3 VP
  keywords:
  - Psionic
  - Ranged
  distance: Ranged 10
  target: Three [[Time Raider|time raiders]]
  effects:
  - name: Effect
    effect: 'Each target is psionically lifted into the air and can [[Fly|fly]] up to their
      speed. If a target doesn’t land in an unoccupied space, they fall. '
- name: Precog Reflexes
  type: Triggered Action
  keywords:
  - Psionic
  - Ranged
  distance: Ranged 10
  target: One creature
  effects:
  - name: '**Trigger**'
    effect: The target attacks the tyrannis.
  - name: Effect
    effect: 'The power roll for the attack takes a bane and the tyrannis makes a free
      strike against the target. '
- name: We Will Won!
  type: Villain Action 1
  keywords:
  - Psionic
  - Ranged
  distance: Ranged 10
  target: Three allies
  effects:
  - name: Effect
    effect: 'Each target gains 15 temporary Stamina and has their speed doubled until
      the end of their turn. '
- name: Stick To The Plan!
  type: Villain Action 2
  keywords:
  - Area
  distance: 10 burst
  target: Each ally
  effects:
  - name: Effect
    effect: 'Each target can end one effect or condition affecting them or can move
      up to their speed. '
- name: Armageddon
  type: Villain Action 3
  keywords:
  - Area
  distance: 5 burst
  target: Special
  effects:
  - name: Effect
    effect: The tyrannis fires a sensor mine into each unoccupied square in the burst
      and a gravity well into one of their own squares. Whenever an enemy moves into
      a square with a sensor mine, the mine explodes, dealing 3 damage to the enemy.

```
