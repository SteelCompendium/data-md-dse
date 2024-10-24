```ds-statblock
name: [[Human]] Storm Mage
ancestry:
- [[Human]]
- Humanoid
roles:
- Controller
level: 3
ev: 17
stamina: 40
immunities:
- Magic 2
- Psionic 2
weaknesses: []
speed: '5'
size: 1M
stability: 0
free_strike: 5
might: 0
intuition: 0
agility: 0
reason: 2
presence: 0
traits:
- name: Arcane Shield
  effect: Whenever the mage takes damage from an enemy adjacent to them, the damage
    is reduced by 3 (minimum 0), and the enemy takes 3 thunder damage and is pushed
    2 squares.
abilities:
- name: Lightning Bolt
  type: Action
  roll: 2d10 + 2
  cost: Signature
  keywords:
  - Attack
  - Magic
  - Ranged
  distance: Ranged 10
  target: One creature or object
  t1: 5 lightning damage
  t2: 8 lightning damage
  t3: 11 lightning damage
- name: Gust of Wind
  type: Maneuver
  roll: MGT RR
  cost: 3 VP
  keywords:
  - Area
  - Magic
  - Resistance
  distance: 5 cube within 1
  target: Each creature and object
  t1: Slide 5; [[Slowed|slowed]] (MGT ends)
  t2: Slide 3; [[Slowed|slowed]] (EoT)
  t3: Slide 1
  effects:
  - name: Effect
    effect: 'The gust of wind disperses gas or vapor and extinguishes any flames,
      including persistent effects. '

```
