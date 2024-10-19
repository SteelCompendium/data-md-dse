```ds-statblock
name: [[Time Raider]] Mind Punk
ancestry:
- Humanoid
- [[Time Raider]]
roles:
- Hexer
level: 3
ev: 17
stamina: 40
immunities:
- Psychic 4
weaknesses: []
speed: '5'
size: '2'
stability: 2
free_strike: 5
might: 2
intuition: 2
agility: 0
reason: 2
presence: 1
traits:
- name: Foresight
  effect: The mind punk doesn’t take a bane on attacks against concealed creatures.
abilities:
- name: Repelling Psihander
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Psionic
  - Weapon
  distance: Reach 1
  target: Two creatures adjacent to each other
  t1: 4 damage
  t2: 6 damage
  t3: 9 damage; [[Dazed|dazed]] (EoT)
  effects:
  - name: Effect
    effect: 'A target who ends their next turn adjacent to the other target falls
      [[Prone|prone]]. '
- name: Mindpunk
  type: Action
  cost: REA RR
  keywords:
  - Area
  - Psionic
  - Resistance
  distance: 2 Burst
  target: All enemies
  t1: 7 psychic damage; push 2; [[Prone|prone]] and can’t stand (EoT)
  t2: 5 psychic damage; push 1
  t3: 2 psychic damage
  effects:
  - name: '**3 VP**'
    effect: 'The size of the burst increases by 1. '

```
