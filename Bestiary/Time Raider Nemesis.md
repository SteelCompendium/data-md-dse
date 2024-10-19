```ds-statblock
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
might: 1
intuition: 1
agility: 2
reason: 2
presence: 0
traits:
- name: Foresight
  effect: The nemesis doesn’t take a bane on attacks against concealed creatures.
abilities:
- name: Golden Scythe
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Psionic
  - Weapon
  distance: Reach 2
  target: One creature or object
  t1: 5 damage
  t2: 8 damage; pull 1
  t3: 11 damage; pull 2; [[Restrained|restrained]] (EoT)
  effects:
  - name: Effect
    effect: 'This ability can affect creatures on parallel planes of existence and
      pull them onto the nemesis’s plane. '
- name: Kinetic Crush
  type: Action
  roll: MGT RR
  cost: 2 VP
  keywords:
  - Psionic
  - Ranged
  - Resistance
  distance: Ranged 10
  target: One creature
  t1: 11 psychic damage; [[Restrained|restrained]] (MGT ends)
  t2: 8 psychic damage; [[Slowed|slowed]] (EoT)
  t3: '5 psychic damage '

```
