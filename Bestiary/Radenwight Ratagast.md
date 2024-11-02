```ds-statblock
name: Radenwight Ratagast
ancestry:
- Humanoid
- Radenwight
roles:
- Defender
- Minion
level: 1
ev: 7
stamina: 12
immunities: []
weaknesses: []
speed: 6 (climb)
size: 1S
stability: 0
free_strike: 2
might: -1
intuition: 0
agility: 1
reason: 0
presence: 2
traits: []
abilities:
- name: Stinky Glissando
  type: Action
  cost: Signature
  keywords:
  - Attack
  - Magic
  - Melee
  distance: Melee 1
  target: One creature or object per minion
  effects:
  - roll: 2d10 + 2
    t1: 2 poison damage
    t2: 4 poison damage; [[Taunted|taunted]] (EoT)
    t3: '5 poison damage; [[Taunted|taunted]] (EoT) '
- name: Ready Rodent
  type: Triggered Action
  keywords:
  - Melee
  - Weapon
  distance: Melee 1
  target: One creature
  trigger: An ally deals damage to the target.
  effects:
  - name: Effect
    effect: The ratagast makes a [[Free Strike|free strike]] against the target.

```
