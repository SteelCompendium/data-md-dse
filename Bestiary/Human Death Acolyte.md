```ds-statblock
name: [[Human]] Death Acolyte
ancestry:
- [[Human]]
- Humanoid
roles:
- Hexer
- Minion
level: 1
ev: 5
stamina: 8
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
presence: 1
traits: []
abilities:
- name: Necrotic Bolt
  type: Action
  roll: 2d10 + 1
  cost: Signature
  keywords:
  - Attack
  - Magic
  - Ranged
  distance: Ranged 10
  target: One creature or object per minion
  t1: 2 corruption damage
  t2: 4 corruption damage
  t3: 5 corruption damage
  effects:
  - name: Effect
    effect: A creature within 5 squares of the death acolyte regains 1 Stamina.

```
