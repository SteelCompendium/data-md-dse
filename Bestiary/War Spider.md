~~~ds-statblock
name: War Spider
ancestry:
- Animal
- Goblin
roles:
- Mount
level: 1
ev: 28
stamina: 60
immunities: []
weaknesses: []
speed: 7 (climb)
size: '3'
stability: 2
free_strike: 4
might: 2
intuition: 0
agility: 1
reason: -4
presence: -3
traits:
- name: Ride Launcher
  effect: An ally who leaps off the back of the spider can jump up to 6 squares without
    a test, and takes no damage if they fall during the jump. After the jump, the
    first melee attack an ally makes on the same turn gains an edge.
- name: Wide Back
  effect: Two of the spider’s size 1 allies can occupy the same space while riding
    the spider.
abilities:
- name: Bite
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Reach 1
  target: One creature or object
  t1: 4 poison damage
  t2: 7 poison damage; weakened (EoT)
  t3: '10 poison damage; weakened (MGT ends) '
- name: Leg Blade
  type: Action
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Reach 1
  target: Two creatures or objects
  t1: 4 damage
  t2: 7 damage
  t3: '10 damage '
- name: Trample
  type: Action
  keywords:
  - —
  distance: Self
  target: Self
  effect: 'The spider shifts up to their speed and makes a Leg Blade attack against
    each creature who comes within their reach during the move. The spider makes one
    power roll against all targets. '
- name: Web
  type: Maneuver
  roll: AGL RR
  cost: 2 VP
  keywords:
  - Area
  - Resistance
  distance: 3 cube within 1
  target: Each creature
  t3: Restrained (AGL ends)
  t2: Restrained (EoT)
  t1: 'No effect '

~~~