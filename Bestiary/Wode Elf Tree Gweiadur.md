```ds-statblock
name: Wode Elf Tree Gweiadur
ancestry:
- Fey
- Humanoid
- Wode Elf
roles:
- Artillery
level: 3
ev: ''
stamina: ''
immunities: []
weaknesses: []
speed: ''
size: ''
stability: ''
free_strike: ''
might: 0
intuition: 1
agility: 2
reason: 0
presence: 0
traits:
- name: Masking Glamor
  effect: The tree gweiadur immediately [[Hide|hides]] at the end of their turn while in cover
    or concealment, even if they are observed.
abilities:
- name: Snare Bow
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Ranged
  - Weapon
  distance: Ranged 15
  target: 1 creature or object
  t1: 5 damage; A1 [[Restrained|restrained]] (save ends)
  t2: 9 damage; A2 [[Restrained|restrained]] (save ends)
  effects:
  - name: Effect
    effect: 'The tree gweiadur can shift 3 after making the attack. 3 Malice: If this
      attack restrains the target, an enemy within 1 of the target is also [[Restrained|restrained]]
      (save ends). '
- name: You Activated My Trap!
  type: Maneuver
  roll: 2d10 + 2
  cost: 3 Malice
  keywords:
  - Area
  - Magic
  - Ranged
  distance: 3 cube within 10
  target: All enemies in the cube
  t1: 2 damage; R1 marked (save ends)
  t2: 4 damage; R2 [[Slowed|slowed]] and marked (save ends)
  effects:
  - name: Effect
    effect: 'Allies have **+1** on attacks and abilities against marked creatures
      and objects. '

```
