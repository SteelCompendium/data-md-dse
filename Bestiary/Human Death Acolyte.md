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
presence: 2
traits:
- name: Supernatural Insight
  effect: The death acolyte can target supernatural creatures and objects within 5
    squares, even if they don't have line of effect.
abilities:
- name: Necrotic Bolt
  type: Action
  cost: Signature
  keywords:
  - Attack
  - Magic
  - Ranged
  distance: Ranged 10
  target: One creature or object per minion
  effects:
  - roll: 2d10 + 2
    t1: 2 corruption damage
    t2: 4 corruption damage
    t3: 5 corruption damage
  - name: Effect
    effect: 'A creature within 5 squares of the death acolyte regains 1 Stamina. '

```
