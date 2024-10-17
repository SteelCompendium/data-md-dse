~~~ds-statblock
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
might: ''
intuition: ''
agility: ''
reason: ''
presence: ''
traits:
- name: Foresight
  effect: The mind punk doesn’t take a bane on attacks against concealed creatures.
abilities:
- name: Repelling Psihander
  type: Action
  roll: 2d10 + 2
  cost: Signature
  t1: 4 damage
  t2: 6 damage
  t3: 9 damage; [[Dazed|dazed]] (EoT)
  effects:
  - name: '**Keywords**'
    effect: Attack, Melee, Psionic, Weapon
  - name: '**Distance**'
    effect: Reach 1
  - name: '**Target**'
    effect: 'Two creatures adjacent to each other '
  - name: '**Effect**'
    effect: 'A target who ends their next turn adjacent to the other target falls
      [[Prone|prone]]. '
- name: Mindpunk
  type: Action
  t3: 7 psychic damage; push 2; [[Prone|prone]] and can’t stand (EoT)
  t2: 5 psychic damage; push 1
  t1: 2 psychic damage
  effects:
  - name: '**Keywords**'
    effect: Area, Psionic, Resistance
  - name: '**Distance**'
    effect: 2 Burst
  - name: '**Target**'
    effect: 'All enemies '
  - name: '**3 VP**'
    effect: 'The size of the burst increases by 1. '

~~~