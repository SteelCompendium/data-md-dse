```ds-statblock
name: Wode Elf Scout
ancestry:
- Fey
- Humanoid
- Wode Elf
roles:
- Ambusher
- Minion
level: 1
ev: 7
stamina: 10
immunities: []
weaknesses: []
speed: '10'
size: 1M
stability: 0
free_strike: 2
might: 0
intuition: 0
agility: 2
reason: 0
presence: 1
traits:
- name: Hunter's Glamor
  effect: The scout immediately [[Hide|hides]] at the end of their turn, even if they are observed.
abilities:
- name: Daggers
  type: Action
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Ranged
  - Weapon
  distance: Melee 1 or Ranged 5
  target: 1 creature or object per minion
  effects:
  - roll: 2d10 + 2
    t1: 2 damage
    t2: 5 damage
    t3: '6 damage '

```
