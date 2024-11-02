```ds-statblock
name: Zombie
ancestry:
- Corporeal
- Undead
roles:
- Brute
level: 1
ev: 10
stamina: 20
immunities:
- Corruption 3
- Poison 3
weaknesses: []
speed: '6'
size: 1M
stability: 1
free_strike: 4
might: 2
intuition: -2
agility: 1
reason: -5
presence: 1
traits:
- name: Arise
  effect: The first time the zombie is reduced to Stamina 0 by damage that isn't fire
    damage or holy damage and their body isn't destroyed, they regain half their Stamina
    and fall [[Prone|prone]].
- name: Endless Knight
  effect: The zombie can take advantage of their Arise trait twice.
abilities:
- name: Clobber and Clutch
  type: Action
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: One creature or object
  effects:
  - roll: 2d10 + 2
    t1: 2 damage; M1 [[Grabbed|grabbed]]
    t2: 5 damage; M2 [[Grabbed|grabbed]]
    t3: 6 damage; [[Grabbed|grabbed]]
  - name: Effect
    effect: 'A target who starts their turn [[Grabbed|grabbed]] by the zombie takes 2 corruption
      damage. If a creature takes 5 or more corruption damage this way, they become
      insatiably hungry for flesh. The target must complete the Find a Cure project
      to end this effect. '
- name: Breakfall
  type: Maneuver
  cost: 3 Malice
  keywords:
  - Area
  - Resistance
  distance: 2 burst
  target: Each enemy in the burst
  effects:
  - roll: 2d10 + 2
    t1: 2 corruption damage
    t2: 3 corruption damage; M1 [[Weakened|weakened]] (save ends)
    t3: '4 corruption damage; M2 [[Dazed|dazed]] (save ends) '

```
