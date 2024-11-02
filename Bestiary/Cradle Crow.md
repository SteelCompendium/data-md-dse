```ds-statblock
name: Cradle Crow
ancestry:
- Construct
- High Elf
roles:
- Harrier
- Minion
level: 1
ev: 6
stamina: 10
immunities: []
weaknesses: []
speed: 7 ([[Fly|fly]])
size: 1T
stability: 0
free_strike: 2
might: 0
intuition: 0
agility: 2
reason: 0
presence: 1
traits: []
abilities:
- name: Heckle
  type: Action
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 1
  target: 1 creature or object per minion
  effects:
  - roll: 2d10 + 2
    t1: 2 damage
    t2: 4 damage; [[Taunted|taunted]] (EoT)
    t3: 5 damage; [[Taunted|taunted]] (EoT)
  - name: Effect
    effect: The cradle crow ignores opportunity attacks from the target until the
      end of its turn.

```
