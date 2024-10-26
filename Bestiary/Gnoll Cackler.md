```ds-statblock
name: Gnoll Cackler
ancestry:
- Fiend
- Gnoll
roles:
- Hexer
level: 2
ev: 11
stamina: 20
immunities: []
weaknesses: []
speed: '5'
size: 1S
stability: 1
free_strike: 3
might: 0
intuition: 2
agility: 0
reason: 2
presence: 2
traits:
- name: Death Frenzy
  effect: Whenever an ally within 5 is reduced to 0 Stamina, the cackler moves up
    to their speed and takes a [[Free Strike|free strike]].
abilities:
- name: Moment of Brutality
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Magic
  - Ranged
  - Resistance
  distance: Ranged 8
  target: 1 creature
  t1: 3 psychic damage; I1 target makes a [[Free Strike|free strike]] against a creature of the cackler’s
    choice
  t2: 5 psychic damage; I2 target makes a [[Free Strike|free strike]] against a creature of the cackler’s
    choice
  effects:
  - name: Effect
    effect: 'An ally targeted by this ability makes a [[Free Strike|free strike]] instead of taking
      damage. '
- name: Cackletongue
  type: Maneuver
  roll: INU RR
  cost: 4 Malice
  keywords:
  - Area
  - Magic
  - Resistance
  distance: 2 burst
  target: All creatures
  t1: [[Frightened]] of the cackler (save ends)
  t2: [[Frightened]] of the cackler (EoT)
  effects:
  - name: Effect
    effect: 'Allies targeted by this ability don’t make a resistance roll. Targets
      who haven’t used a cackletongue maneuver on this turn use it immediately at
      no cost. '

```
