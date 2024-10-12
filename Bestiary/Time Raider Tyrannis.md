~~~ds-statblock
name: Time Raider Tyrannis
ancestry:
- Humanoid
- Time Raider
roles:
- Boss
level: 3
ev: 54
stamina: 120
immunities:
- Psychic 7
weaknesses: []
speed: 10 (fly, teleport)
size: '2'
stability: 0
free_strike: 5
might: ''
intuition: ''
agility: ''
reason: ''
presence: ''
traits:
- name: End Effect
  effect: At the end of their turn, the tyrannis can take 5 damage to end one EoE
    effect affecting them. This damage can’t be reduced in any way.
- name: Foresight
  effect: The tyrannis doesn’t take a bane on attacks against concealed creatures.
abilities:
- name: Gatling Blaster
  type: Action
  roll: 2d10 + 3
  cost: Signature
  t1: 5 corruption damage
  t2: 9 corruption damage
  t3: 12 corruption damage
- name: Air Raid!
  type: Maneuver
- name: Precog Reflexes
  type: Triggered Action
- name: We Will Won!
  type: Villain Action
  cost: 1 VP
- name: Stick To The Plan!
  type: Villain Action
  cost: 2 VP
- name: Armageddon
  type: Villain Action
  cost: 3 VP

~~~