```ds-statblock
name: [[Human]] [[Raider]]
ancestry:
- [[Human]]
- Humanoid
roles:
- Harrier
- Minion
level: 1
ev: 6
stamina: 10
immunities:
- Magic 2
- Psionic 2
weaknesses: []
speed: '7'
size: 1M
stability: 0
free_strike: 2
might: 0
intuition: 0
agility: 2
reason: 0
presence: 0
traits:
- name: Supernatural Insight
  effect: The [[Raider|raider]] can target supernatural creatures and objects within 5 squares,
    even if they don't have line of effect.
abilities:
- name: Handaxes
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
  target: One creature or object per minion
  t1: 2 damage
  t2: 4 damage
  t3: 5 damage
  effects:
  - name: Effect
    effect: 'If this ability is used while Charging, the [[Raider|raider]] can make a ranged
      [[Free Strike|free strike]] with a distance of 5 before using the ability. '

```
