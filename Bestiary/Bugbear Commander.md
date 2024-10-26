```ds-statblock
name: Bugbear Commander
ancestry: []
roles: []
level: ''
ev: 32
stamina: 70
immunities: []
weaknesses: []
speed: '5'
size: 1M
stability: 0
free_strike: 5
might: 2
intuition: 0
agility: 1
reason: 2
presence: 0
traits:
- name: LEVEL 2 SUPPORT
  effect: '*Bugbear, Goblin, Humanoid*'
- name: Catcher (Free Triggered Action)
  effect: 'Keywords: — Distance: Melee 1 Target: 1 size 1 creature or object Trigger:
    The target is force moved into a square adjacent to the commander. - Effect: The
    target is [[Grabbed|grabbed]] by the commander.'
- name: The Commander’s Watching
  effect: While an ally has line of effect to the commander, the ally can end one
    condition afflicting them at the start of their turn.
abilities:
- name: Inspiring Swordplay
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: 2 creatures or objects
  t1: 5 damage
  t2: 8 damage
  t3: 11 damage; one target is [[Grabbed|grabbed]]
- name: You Next!
  type: Action
  keywords:
  - —
  distance: Ranged 8
  target: 1 ally
- name: Fall Back!
  type: Action
  cost: 5 Malice
  keywords:
  - —
  distance: Self and 5 burst
  target: Self and all allies
- name: Throw
  type: Maneuver
  keywords:
  - Attack
  - Melee
  distance: Melee 1
  target: 1 creature or object [[Grabbed|grabbed]] by the commander

```
