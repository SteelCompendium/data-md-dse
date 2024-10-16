~~~ds-statblock
name: [[Time Raider]] Armiger
ancestry:
- Humanoid
- [[Time Raider]]
roles:
- Defender
level: 3
ev: 21
stamina: 60
immunities:
- Psychic 5
weaknesses: []
speed: '5'
size: 1M
stability: 0
free_strike: 5
might: ''
intuition: ''
agility: ''
reason: ''
presence: ''
traits:
- name: Foresight
  effect: The armiger doesn’t take a bane on attacks against concealed creatures.
- name: Kuran’zoi Heraldry
  effect: While any [[Time Raider|time raider]] starts their turn with line of effect to the armiger,
    that [[Time Raider|time raider]] can end one condition affecting them.
abilities:
- name: Serrated Saber
  type: Action
  roll: 2d10 + 2
  cost: Signature
  t1: 5 damage
  t2: 8 damage; [[Weakened|weakened]] (EoT)
  t3: 11 damage; [[Weakened|weakened]] (REA ends)
- name: Shared Sickness
  type: Triggered Action
  t3: 11 poison damage
  t2: 8 poison damage
  t1: '5 poison damage '

~~~