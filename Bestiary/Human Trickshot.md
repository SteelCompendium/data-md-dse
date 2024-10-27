```ds-statblock
name: [[Human]] Trickshot
ancestry:
- [[Human]]
- Humanoid
roles:
- Artillery
level: 1
ev: 12
stamina: 20
immunities:
- Magic 2
- Psionic 2
weaknesses: []
speed: '5'
size: 1M
stability: 0
free_strike: 4
might: 0
intuition: 1
agility: 2
reason: 0
presence: 0
traits:
- name: Supernatural Insight
  effect: The trickshot can target supernatural creatures and objects within 5 squares,
    even if they don't have line of effect.
abilities:
- name: Trick Crossbow
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Ranged
  - Weapon
  distance: Melee 1 or Ranged 15
  target: One creature or object
  t1: 4 damage
  t2: 7 damage
  t3: 10 damage
  effects:
  - name: Effect
    effect: The trickshot ignores cover and concealment.
  - name: 3 Malice
    effect: 'The trickshot attacks an additional target. '

```
