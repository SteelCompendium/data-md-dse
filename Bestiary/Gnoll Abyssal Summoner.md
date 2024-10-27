```ds-statblock
name: Gnoll Abyssal Summoner
ancestry:
- Fiend
- Gnoll
roles:
- Support
level: 2
ev: 12
stamina: 25
immunities: []
weaknesses: []
speed: '5'
size: 1M
stability: 1
free_strike: 3
might: 1
intuition: 2
agility: 0
reason: 0
presence: 2
traits:
- name: Death Frenzy
  effect: Whenever an ally within 5 is reduced to 0 Stamina, the abyssal summoner
    moves up to their speed and makes a [[Free Strike|free strike]].
abilities:
- name: Flame Wad
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Magic
  - Ranged
  distance: Ranged 5
  target: 1 creature or object
  t1: 3 fire damage; I1 burning (save ends)
  t2: 5 fire damage; I2 burning (save ends)
  effects:
  - name: Effect
    effect: 'A burning target takes 1d6 fire damage at the start of each of their
      turns until the condition ends. '
- name: Call [[Abyssal Hyena|Abyssal Hyenas]]
  type: Maneuver
  cost: 3 Malice
  keywords:
  - '-'
  distance: Ranged 5
  target: Special
  effects:
  - name: Effect
    effect: '2 [[Abyssal Hyena|abyssal hyenas]] claw out of the ground into unoccupied squares. '
- name: Cackletongue
  type: Maneuver
  cost: 4 Malice
  keywords:
  - '-'
  distance: 2 burst
  target: All allies
  effects:
  - name: Effect
    effect: '1 [[Abyssal Hyena|abyssal hyena]] target turns into a [[Gnoll Marauder|gnoll marauder]], keeping their Stamina.
      Targets who haven''t used a cackletongue maneuver on this turn use it immediately
      at no cost. '

```
