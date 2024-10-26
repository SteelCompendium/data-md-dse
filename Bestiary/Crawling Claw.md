```ds-statblock
name: Crawling Claw
ancestry:
- Corporeal
- Undead
roles:
- Harrier
- Minion
level: 1
ev: 2
stamina: 5
immunities:
- Corruption 2
- Poison 2
weaknesses: []
speed: 6 (climb)
size: 1T
stability: 0
free_strike: 1
might: 0
intuition: -1
agility: 2
reason: -5
presence: -1
traits:
- name: Disorganized
  effect: The crawling claw can’t grant the flanking benefit to allies.
abilities:
- name: Fingernails
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: One creature or object per minion
  t1: 1 damage
  t2: 2 damage
  t3: 3 damage
  effects:
  - name: Effect
    effect: 'The crawling claw shifts a number of squares equal to the damage dealt. '

```
