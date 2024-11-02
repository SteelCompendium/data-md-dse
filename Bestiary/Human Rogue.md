```ds-statblock
name: [[Human]] Rogue
ancestry:
- [[Human]]
- Humanoid
roles:
- Ambusher
- Minion
level: 1
ev: 7
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
presence: 1
traits:
- name: Supernatural Insight
  effect: The rogue can target supernatural creatures and objects within 5 squares,
    even if they don't have line of effect.
abilities:
- name: Concealed Dagger
  type: Action
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Ranged
  - Weapon
  distance: Melee 1 or Ranged 5
  target: One creature or object per minion
  effects:
  - roll: 2d10 + 2
    t1: 2 damage
    t2: 5 damage
    t3: 6 damage
  - name: Effect
    effect: 'This attack has a double edge and an edge if the spy was disguised or
      hidden before using this ability. '

```
