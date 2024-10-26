```ds-statblock
name: Wode Elf Tree Chirurgeon
ancestry:
- Fey
- Humanoid
- Wode Elf
roles:
- Harrier
level: 2
ev: ''
stamina: ''
immunities: []
weaknesses: []
speed: ''
size: ''
stability: ''
free_strike: ''
might: 1
intuition: 0
agility: 2
reason: 0
presence: 0
traits:
- name: Masking Glamor
  effect: The tree chirurgeon immediately [[Hide|hides]] at the end of their turn while in
    cover or concealment, even if they are observed.
abilities:
- name: Wild Axe
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - [[Charge]]
  - Melee
  - Ranged
  - Weapon
  distance: Melee 1 or Ranged 5
  target: 1 creature or object
  t1: 4 damage; push 1
  t2: 7 damage; push 3
  effects:
  - name: Effect
    effect: 'The tree chirurgeon can make a ranged [[Free Strike|free strike]] before attacking. 5
      Malice: The tree chirurgeon uses this ability again. '
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
