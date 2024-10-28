```ds-statblock
name: Lizardfolk Scaletooth
ancestry:
- Humanoid
- Lizardfolk
roles:
- Brute
level: 1
ev: 16
stamina: 40
immunities:
- weapon 3
weaknesses: []
speed: 5 (swim)
size: 1M
stability: 0
free_strike: 5
might: 2
intuition: ''
agility: 1
reason: 0
presence: 0
traits:
- name: Reptilian Escape
  effect: While the scaletooth still has a tail, whenever the scaletooth is [[Grabbed|grabbed]],
    [[Slowed|slowed]], [[Weakened|weakened]], or knocked [[Prone|prone]], the scaletooth can lose their tail to immediately
    end the effect and shift 2.
abilities:
- name: Razor Bite
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: 1 creature or object
  t1: 5 damage; A1 [[Bleeding|bleeding]] (save ends)
  t2: 9 damage; A2 [[Bleeding|bleeding]] (save ends)
  t3: 12 damage; A3 [[Bleeding|bleeding]] (save ends)
  effects:
  - name: Effect
    effect: 'The potency of this attack increases by 1 if the target is [[Grabbed|grabbed]] by
      the scaletooth. '
- name: Tail Whip
  type: Action
  roll: 2d10 + 2
  cost: 2 Malice
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 2
  target: 2 creatures or objects
  t1: 3 damage; slide 1; M1 grappled
  t2: 5 damage; slide 2; M2 grappled
  t3: 6 damage; slide 3; M3 grappled if within 2 of the scaletooth
  effects:
  - name: Effect
    effect: 'The scaletooth needs their tail to use this ability. The scaletooth can''t
      grapple more than one creature or object with this ability. '

```
