```ds-statblock
name: [[Human]] Scoundrel
ancestry:
- [[Human]]
- Humanoid
roles:
- Ambusher
level: 1
ev: 14
stamina: 30
immunities:
- Magic 2
- Psionic 2
weaknesses: []
speed: '5'
size: 1M
stability: 0
free_strike: 4
might: 0
intuition: 0
agility: 2
reason: 0
presence: 1
traits:
- name: Supernatural Insight
  effect: The scoundrel can target supernatural creatures and objects within 5 squares,
    even if they don't have line of effect.
abilities:
- name: Rapier & Dagger
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: One creature or object
  t1: 4 damage
  t2: 7 damage
  t3: 10 damage
  effects:
  - roll: 2d10 + 2
    t1: 4 damage
    t2: 7 damage
    t3: 10 damage
  - name: Effect
    effect: 'This ability has double edge if the scoundrel has an edge on the power
      roll. '
- name: Dagger Storm
  type: Action
  cost: 5 Malice

```
