```ds-statblock
name: [[Human]] Apprentice Mage
ancestry:
- [[Human]]
- Humanoid
roles:
- Controller
- Minion
level: 2
ev: 6
stamina: 10
immunities:
- Magic 2
- Psionic 2
weaknesses: []
speed: '5'
size: 1M
stability: 0
free_strike: 2
might: 0
intuition: 0
agility: 1
reason: 0
presence: 2
traits:
- name: Studied Supernatural Insight
  effect: The apprentice can target supernatural creatures and objects within 10 squares,
    even if they don’t have line of effect.
abilities:
- name: Lightning Strike
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Magic
  - Ranged
  distance: Ranged 10
  target: One creature or object per minion
  t1: 2 lightning damage
  t2: 4 lightning damage
  t3: 5 lightning damage
  effects:
  - name: Effect
    effect: 'If the apprentice mage doesn’t use a maneuver or a move action this turn,
      the target is [[Slowed|slowed]] (EoT). '

```
