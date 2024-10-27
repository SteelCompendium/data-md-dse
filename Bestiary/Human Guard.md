```ds-statblock
name: [[Human]] Guard
ancestry:
- [[Human]]
- Humanoid
roles:
- Brute
- Minion
level: 1
ev: 6
stamina: 12
immunities:
- Magic 2
- Psionic 2
weaknesses: []
speed: '5'
size: 1M
stability: 0
free_strike: 2
might: 2
intuition: 0
agility: 0
reason: 0
presence: 0
traits:
- name: Supernatural Insight
  effect: The guard can target supernatural creatures and objects within 5 squares,
    even if they don't have line of effect.
abilities:
- name: Halberd
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 2
  target: One creature or object per minion
  t1: 2 damage
  t2: 5 damage
  t3: 6 damage
  effects:
  - name: Effect
    effect: 'If the guard is flanked, they can make a [[Free Strike|free strike]] against an additional
      target adjacent to them. '

```
