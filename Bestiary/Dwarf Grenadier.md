```ds-statblock
name: [[Dwarf]] Grenadier
ancestry:
- [[Dwarf]]
- Humanoid
roles:
- Hexer
level: 2
ev: 13
stamina: 33
immunities: []
weaknesses: []
speed: '5'
size: 1M
stability: 3
free_strike: 4
might: 1
intuition: 2
agility: 0
reason: 0
presence: 0
traits:
- name: Indirect Fire
  effect: The grenadier ignores cover and concealment and doesn't need to establish
    line of effect for their abilities.
abilities:
- name: Concussive Grenade
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Area
  - Ranged
  - Weapon
  distance: 3 cube within 5
  target: All enemies
  t1: 3 damage; push 1; M1 [[Slowed|slowed]] (save ends)
  t2: 5 damage; push 3; M2 [[Slowed|slowed]] (save ends)
  t3: 7 damage; push 5; M3 [[Slowed|slowed]] (save ends)
  effects:
  - roll: 2d10 + 2
    t1: 3 damage; push 1; M1 [[Slowed|slowed]] (save ends)
    t2: 5 damage; push 3; M2 [[Slowed|slowed]] (save ends)
    t3: 7 damage; push 5; M3 [[Slowed|slowed]] (save ends)
  - name: Effect
    effect: 'A target [[Restrained|restrained]] by a [[Dwarf|dwarf]] can be pushed by this ability. '
- name: Sleep Grenade
  type: Action
  roll: 2d10 + 2
  cost: 3 Malice
  keywords:
  - Area
  - Ranged
  distance: 3 cube within 5
  target: All enemies
  t1: 3 poison damage; I1 [[Dazed|dazed]] (save ends)
  t2: 5 poison damage; I2 [[Dazed|dazed]] (save ends)
  t3: 7 poison damage; I3 [[Dazed|dazed]] (save ends)
  effects:
  - roll: 2d10 + 2
    t1: 3 poison damage; I1 [[Dazed|dazed]] (save ends)
    t2: 5 poison damage; I2 [[Dazed|dazed]] (save ends)
    t3: 7 poison damage; I3 [[Dazed|dazed]] (save ends)
  - name: Effect
    effect: 'A creature [[Dazed|dazed]] by this ability has -1 to all characteristics while
      resisting potent effects until the condition ends. '

```
