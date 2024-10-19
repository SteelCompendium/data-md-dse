```ds-statblock
name: War Dog Portalite
ancestry:
- Humanoid
- War Dog
roles:
- Ambusher
level: 1
ev: 11
stamina: 20
immunities: []
weaknesses: []
speed: 5 ([[Teleport|teleport]])
size: 1M
stability: 0
free_strike: 3
might: 0
intuition: 0
agility: 1
reason: 0
presence: 0
traits:
- name: Loyalty Collar
  effect: When the portalite dies, they explode, dealing 1d6 damage to each adjacent
    enemy.
abilities:
- name: Corrupted Ash Daggers
  type: Action
  roll: 2d10 + 1
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Ranged
  - Weapon
  distance: Reach 1 or Ranged 5
  target: One creature or object
  t1: 3 damage; slide 1
  t2: 5 damage; slide 2
  t3: 7 damage; slide 3
  effects:
  - name: Effect
    effect: The power roll gains an edge if any of the portalite’s allies are adjacent
      to the target.
  - name: '**1 VP**'
    effect: 'The portalite [[Teleport|teleports]] the target up to 3 squares before sliding them. '
- name: Posthumous Promotion
  type: Maneuver
  keywords:
  - Magic
  - Ranged
  distance: Ranged 10
  target: One war dog with a loyalty collar
  effects:
  - name: Effect
    effect: 'The target’s loyalty collar detonates, killing them instantly. '
- name: Corrupted Ash [[Teleport]] (Maneuver) ◆ 1 VP
  keywords:
  - Magic
  distance: Self
  target: Self
  effects:
  - name: Effect
    effect: 'The portalite [[Teleport|teleports]] up to 5 squares and gains an edge on attacks
      this turn. '

```
