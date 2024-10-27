```ds-statblock
name: [[Dwarf]] Trapper
ancestry:
- [[Dwarf]]
- Humanoid
roles:
- Harrier
level: 1
ev: 13
stamina: 36
immunities: []
weaknesses: []
speed: '7'
size: 1M
stability: 2
free_strike: 3
might: 0
intuition: 1
agility: 2
reason: 0
presence: 0
traits: []
abilities:
- name: Concussive Bolts
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - [[Charge]]
  - Melee
  - Ranged
  - Weapon
  distance: Melee 1 or Ranged 10
  target: 1 creature or object
  t1: 3 damage; push 2
  t2: 5 damage; push 4
  effects:
  - name: Effect
    effect: 'A target [[Restrained|restrained]] by a [[Dwarf|dwarf]] can be pushed by this attack. '
- name: Steam Powered Snare
  type: Maneuver
  roll: MGT RR
  cost: 3 Malice
  keywords:
  - Area
  - Resistance
  distance: 3 cube within 5
  target: All enemies in the cube
  t1: 4 damage; [[Restrained|restrained]] (EoT)
  t2: 3 damage; [[Slowed|slowed]] (EoT)
  effects:
  - name: Effect
    effect: The snare remains until the end of the encounter. An enemy that moves
      into an affected square for the first time on their turn must roll resistance.

```
