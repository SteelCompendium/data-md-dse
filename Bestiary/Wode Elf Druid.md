```ds-statblock
name: Wode Elf Druid
ancestry:
- Fey
- Humanoid
- Wode Elf
roles:
- Controller
level: 2
ev: ''
stamina: ''
immunities: []
weaknesses: []
speed: ''
size: ''
stability: ''
free_strike: ''
might: 0
intuition: 0
agility: 1
reason: 0
presence: 2
traits:
- name: Masking Glamor
  effect: The druid immediately [[Hide|hides]] at the end of their turn while in cover or concealment,
    even if they are observed.
abilities:
- name: Entangling Vines
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Area
  - Magic
  - Ranged
  distance: 3 cube within 10
  target: All enemies in the cube
  t1: 3 damage; pull 1; M1 [[Slowed|slowed]] (save ends)
  t2: 5 damage; pull 3; M2 [[Slowed|slowed]] (save ends)
  t3: 7 damage; pull 5; M3 [[Slowed|slowed]] (save ends)
  effects:
  - name: Effect
    effect: A creature [[Slowed|slowed]] by this ability can't [[Search For Hidden Creatures|search for hidden creatures]] until
      the condition ends.
  - name: 3 Malice
    effect: 'The area of the cube and the potency of the effect both increase by 1. '
- name: The Wode Protects Us
  type: Maneuver
  cost: 3 Malice
  keywords:
  - Magic
  distance: Self and Ranged 5
  target: Self and 3 allies
  effects:
  - name: Effect
    effect: 'Each target [[Teleport|teleports]] to a square within 10 that has cover or concealment
      from all enemies. '

```
