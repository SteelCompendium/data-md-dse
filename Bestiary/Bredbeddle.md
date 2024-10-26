```ds-statblock
name: Bredbeddle
ancestry: []
roles: []
level: ''
ev: 88
stamina: 240
immunities: []
weaknesses: []
speed: '5'
size: '2'
stability: 4
free_strike: 6
might: 3
intuition: 0
agility: 0
reason: -3
presence: 2
traits:
- name: LEVEL 3 SOLO
  effect: '*Giant*'
- name: Solo Monster
  effect: ''
- name: Resilient Form
  effect: The bredbeddle can’t be physically transformed in any way except by their
    Heady or Not trait.
- name: Heady or Not
  effect: While headless, the bredbeddle can move into a space with a severed head
    and attach it to their neck. Doing so physically transforms the bredbeddle, who
    takes on the size, weight, reach, and stability of the head’s original owner.
    These effects last until the bredbeddle is killed or beheaded, or until the head
    falls off after 24 hours. A head that falls off can no longer be attached to the
    bredbeddle.  A creature must succeed on a hard Might test made as a maneuver to
    rip a head off the bredbeddle. If they fail, the bredbeddle can use Executioner’s
    Swing against them.
abilities:
- name: Executioner’s Swing
  type: Action
  roll: 2d10 + 3
  cost: Signature
  keywords:
  - Area
  - Resistance
  - Weapon
  distance: 2 burst
  target: Each enemy in the burst
  t1: 2 damage; A2 [[Bleeding|bleeding]] (save ends)
  t2: 4 damage; A3 [[Bleeding|bleeding]] (save ends)
  t3: 5 damage; A4 [[Bleeding|bleeding]] and [[Dazed|dazed]] (save ends)
- name: Lop
  type: Action
  roll: 2d10 + 3
  cost: 3 Malice
  keywords:
  - Attack
  - Magic
  - Melee
  - Weapon
  distance: Melee 2
  target: One creature
  t1: 6 damage; [[Bleeding|bleeding]] (save ends) or M2 beheaded (see effect)
  t2: 10 damage; [[Bleeding|bleeding]] (save ends) or M3 beheaded (see effect)
  t3: 13 damage; [[Bleeding|bleeding]] (save ends) or M4 beheaded (see effect)
- name: Scramble
  type: Maneuver
  keywords:
  - —
  distance: Self
  target: Self
- name: Headway
  type: Maneuver
  roll: 2d10 + 3
  cost: 5 Malice
  keywords:
  - Attack
  - Ranged
  - Weapon
  distance: Ranged 20
  target: One creature or object
  t1: 3 damage; M2 [[Dazed|dazed]] (save ends)
  t2: 5 damage; [[Prone|prone]]; M3 [[Dazed|dazed]] (save ends)
  t3: '7 damage; [[Prone|prone]]; M4 [[Dazed|dazed]] (save ends) '
- name: Rebuke of the Fiendish Burlow
  type: Triggered Action
  cost: 2 Malice
  keywords:
  - Magic
  distance: Self
  target: Self
  trigger: A creature targets the bredbeddle with a ranged magic attack.
- name: Turn Green
  type: Villain Action 1
  cost: PRS RR
  keywords:
  - Area
  - Magic
  - Resistance
  distance: 3 burst
  target: Each enemy in the burst
  t1: The target turns green and is [[Slowed|slowed]] (save ends)
  t2: The target turns green (save ends)
  t3: 'No effect '
- name: Challenge
  type: Villain Action 2
  keywords:
  - —
  distance: Ranged 5
  target: One creature who damaged the bredbeddle this encounter
- name: Headlam Rampage
  type: Villain Action 3
  cost: 2d10 + 3
  keywords:
  - Attack
  - Melee
  - Weapon
  distance: Melee 2
  target: Four creatures
  t1: 3 damage; [[Bleeding|bleeding]] (save ends) or M2 beheaded (see Lop)
  t2: 4 damage; [[Bleeding|bleeding]] (save ends) or M3 beheaded (see Lop)
  t3: 5 damage; [[Bleeding|bleeding]] (save ends) or M4 beheaded (see Lop)

```
