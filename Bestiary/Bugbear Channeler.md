```ds-statblock
name: Bugbear Channeler
ancestry: []
roles: []
level: ''
ev: 30
stamina: 60
immunities: []
weaknesses: []
speed: '5'
size: 1M
stability: 0
free_strike: 5
might: 1
intuition: 0
agility: 1
reason: 2
presence: 2
traits:
- name: LEVEL 2 CONTROLLER
  effect: '*Bugbear, Goblin, Humanoid*'
- name: Catcher (Free Triggered Action)
  effect: 'Keywords: — Distance: Melee 1 Target: 1 size 1 creature or object Trigger:
    The target is force moved into a square adjacent to the channeler. - Effect: The
    target is [[Grabbed|grabbed]] by the channeler.'
abilities:
- name: Shape Earth
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Magic
  - Ranged
  distance: Ranged 8
  target: 2 creatures or objects on the ground
  t1: 5 damage; pull 2
  t2: 8 damage; pull 3
  t3: 11 damage; pull 4
- name: Blistering Element
  type: Action
  cost: 2d10 + 2
  keywords:
  - Area
  - Magic
  distance: 3 burst
  target: All enemies in the burst
  t1: 2 damage; M1 [[Bleeding|bleeding]] (save ends)
  t2: 3 damage; M2 [[Bleeding|bleeding]] (save ends)
  t3: 4 damage; M3 [[Bleeding|bleeding]] (save ends)
- name: Green Reshape
  type: Action
  roll: 2d10 + 2
  cost: 5 Malice
  keywords:
  - Magic
  - Ranged
  - Resistance
  distance: Ranged 5
  target: 1 creature
  t1: 5 damage; P1 [[Slowed|slowed]] (save ends)
  t2: 8 damage; P2 shapechanged (save ends)
  t3: 11 damage; P3 shapechanged (save ends)
- name: Throw
  type: Maneuver
  keywords:
  - Attack
  - Melee
  distance: Melee 1
  target: 1 creature or object [[Grabbed|grabbed]] by the channeler
- name: Brambleguard
  type: Triggered Action
  cost: 1 Malice
  keywords:
  - Magic
  - Ranged
  distance: Ranged 5
  target: 1 ally
  trigger: The target takes non-fire damage.

```
