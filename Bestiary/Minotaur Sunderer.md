```ds-statblock
"name": "[[Minotaur]] Sunderer"
"ancestry":
- "[[Minotaur]]"
- "Monster"
"roles":
- "Brute"
"level": !!int "3"
"ev": !!int "40"
"stamina": !!int "90"
"immunities": []
"weaknesses": []
"speed": "6"
"size": "2"
"stability": !!int "2"
"free_strike": !!int "6"
"might": !!int "2"
"intuition": !!int "2"
"agility": !!int "1"
"reason": !!int "0"
"presence": !!int "-1"
"traits":
- "name": "[[Minotaur]] Sense"
  "effect": "The sunderer cannot get a result lower than tier 2 when making Tests\
    \ to navigate, search, or seek."
"abilities":
- "name": "Spiked Maul"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Charge"
  - "Melee"
  - "Weapon"
  "distance": "Melee 2"
  "target": "2 creatures or objects"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "6 damage; pull 1"
    "t2": "10 damage; pull 2"
    "t3": "13 damage; pull 3"
  - "name": "Effect"
    "effect": "A target is grabbed if they are pulled adjacent to the sunderer. "
- "name": "Fearsome Bay"
  "type": "Action"
  "cost": "5 Malice"
  "keywords":
  - "Area"
  - "Resistance"
  "distance": "3 burst"
  "target": "All enemies in the burst"
  "effects":
  - "roll": "INU RR"
    "t1": "Frightened of the [[Minotaur|minotaur]] (save ends)"
    "t2": "Frightened of the [[Minotaur|minotaur]] (EoT)"
    "t3": "No effect"
  - "name": "Effect"
    "effect": "The [[Minotaur|minotaur]] has **resistance** and **advantage** until the end of\
      \ their next turn. "
- "name": "Disemboweling Horns"
  "type": "Maneuver"
  "cost": "3 Malice"
  "keywords":
  - "Attack"
  - "Charge"
  - "Melee"
  - "Weapon"
  "distance": "Melee 2"
  "target": "1 grabbed creature"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "6 damage; push 1; M1 bleeding (save ends)"
    "t2": "10 damage; push 3; M2 bleeding (save ends)"
    "t3": "13 damage; push 5; M3 bleeding (save ends)"
  - "name": "Effect"
    "effect": "The target takes 6 damage at the start of each of their turns while\
      \ bleeding from this ability. "
- "name": "Retaliatory Gore"
  "type": "Triggered Action"
  "keywords":
  - "--"
  "trigger": "The sunderer takes damage from a creature within 6."
  "distance": "Self"
  "target": "Triggering creature"
  "effects":
  - "name": "Effect"
    "effect": "The sunderer charges the target using Spiked Maul. "

```
