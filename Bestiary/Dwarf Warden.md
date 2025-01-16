```ds-statblock
"name": "Dwarf Warden"
"ancestry":
- "Dwarf"
- "Humanoid"
"roles":
- "Brute"
"level": !!int "2"
"ev": !!int "18"
"stamina": !!int "53"
"immunities": []
"weaknesses": []
"speed": "5"
"size": "1M"
"stability": !!int "3"
"free_strike": !!int "5"
"might": !!int "2"
"intuition": !!int "1"
"agility": !!int "0"
"reason": !!int "0"
"presence": !!int "0"
"traits":
- "name": "Escort the Prisoners"
  "effect": "Whenever the warden moves, they can carry an adjacent restrained enemy\
    \ as if they were grabbed."
"abilities":
- "name": "Concussive Maul"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "Melee 1"
  "target": "1 creature or object"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "5 damage; push 1; M1 slowed (save ends)"
    "t2": "8 damage; push 3; M2 slowed (save ends)"
    "t3": "11 damage; push 5; M3 restrained (save ends)"
  - "name": "Effect"
    "effect": "A target restrained by a dwarf can be pushed by this attack. "
- "name": "Concussive Shockwave"
  "type": "Maneuver"
  "cost": "5 Malice"
  "keywords":
  - "Area"
  "distance": "3 cube within 1"
  "target": "All enemies in the cube"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage; push 2; A1 slowed (save ends)"
    "t2": "4 damage; push 4; A2 slowed (save ends)"
    "t3": "5 damage; push 6; A3 dazed (save ends)"
  - "name": "Effect"
    "effect": "A target restrained by a dwarf can be pushed by this ability. "

```
