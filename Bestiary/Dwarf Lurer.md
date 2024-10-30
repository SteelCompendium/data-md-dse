```ds-statblock
name: [[Dwarf]] Lurer
ancestry:
- [[Dwarf]]
- Humanoid
roles:
- Defender
- Minion
level: 1
ev: 7
stamina: 14
immunities: []
weaknesses: []
speed: '5'
size: 1M
stability: 2
free_strike: 2
might: 1
intuition: 2
agility: 0
reason: 0
presence: 0
traits: []
abilities:
- name: Whistling Axes
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Ranged
  - Weapon
  distance: Melee 1 or Ranged 5
  target: 1 creature or object per minion
  t1: 2 damage
  t2: 4 damage
  t3: 5 damage; an ally adjacent to the target can make a [[Free Strike|free strike]]
  effects:
  - roll: 2d10 + 2
    t1: 2 damage
    t2: 4 damage
    t3: 5 damage; an ally adjacent to the target can make a [[Free Strike|free strike]]
  - name: Effect
    effect: The target can't use triggered actions until the start of the next round.

```
