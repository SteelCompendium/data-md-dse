~~~ds-statblock
name: [[Time Raider]] Nemesis
ancestry:
- Humanoid
- [[Time Raider]]
roles:
- Harrier
level: 3
ev: 19
stamina: 50
immunities:
- Psychic 5
weaknesses: []
speed: '7'
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
  effect: The nemesis doesn’t take a bane on attacks against concealed creatures.
abilities:
- name: Golden Scythe
  type: Action
  roll: 2d10 + 2
  cost: Signature
  t1: 5 damage
  t2: 8 damage; pull 1
  t3: 11 damage; pull 2; [[Restrained|restrained]] (EoT)
  effects:
  - name: '**Keywords**'
    effect: Attack, Melee, Psionic, Weapon
  - name: '**Distance**'
    effect: Reach 2
  - name: '**Target**'
    effect: 'One creature or object '
  - name: '**Effect**'
    effect: 'This ability can affect creatures on parallel planes of existence and
      pull them onto the nemesis’s plane. '
- name: Kinetic Crush
  type: Action
  roll: MGT RR
  cost: 2 VP
  t3: 11 psychic damage; [[Restrained|restrained]] (MGT ends)
  t2: 8 psychic damage; [[Slowed|slowed]] (EoT)
  t1: '5 psychic damage '
  effects:
  - name: '**Keywords**'
    effect: Psionic, Ranged, Resistance
  - name: '**Distance**'
    effect: Ranged 10
  - name: '**Target**'
    effect: 'One creature '

~~~