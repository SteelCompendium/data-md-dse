```ds-statblock
name: Wode Elf Tree Guerilla
ancestry:
- Fey
- Humanoid
- Wode Elf
roles:
- Ambusher
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
intuition: 0
agility: 2
reason: 0
presence: 1
traits:
- name: Hunter's Glamor
  effect: The tree guerilla immediately [[Hide|hides]] at the end of their turn, even if they
    are observed.
abilities:
- name: Splinter Dagger
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Ranged
  - Weapon
  distance: Melee 1 or Ranged 5
  target: 1 creature or object
  t1: 5 damage; M1 [[Bleeding|bleeding]] (save ends)
  t2: 9 damage; M2 [[Bleeding|bleeding]] (save ends)
  t3: 12 damage; M3 [[Bleeding|bleeding]] (save ends)
  effects:
  - name: Effect
    effect: The tree guerilla can [[Teleport|teleport]] 3 after making the attack.
  - name: 5 Malice
    effect: 'The tree guerilla targets an additional creature or object. The tree
      guerilla has **+1** if both targets are adjacent to each other. '
- name: Do Not Hesitate in the Wode
  type: Free Triggered Action
  cost: 3 Malice
  keywords:
  - '-'
  distance: Self and Squad
  target: Self and Squad
  trigger: An ally ends their turn while the tree guerilla hasn't acted this round.
  effects:
  - name: Effect
    effect: 'The targets take their turn immediately. Each target has **+1** until
      the end of their turn. '

```
