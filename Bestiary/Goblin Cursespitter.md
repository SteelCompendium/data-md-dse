```ds-statblock
"name": "Goblin Cursespitter"
"ancestry":
- "Goblin"
- "Humanoid"
"roles":
- "Hexer"
"level": !!int "1"
"ev": !!int "9"
"stamina": !!int "15"
"immunities": []
"weaknesses": []
"speed": "5 (climb)"
"size": "1S"
"stability": !!int "0"
"free_strike": !!int "2"
"might": !!int "-2"
"intuition": !!int "2"
"agility": !!int "1"
"reason": !!int "0"
"presence": !!int "0"
"traits":
- "name": "Crafty"
  "effect": "The cursespitter doesn't provoke opportunity attacks by moving."
"abilities":
- "name": "Eye of Surlach"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Magic"
  - "Ranged"
  - "Resistance"
  "distance": "Ranged 10"
  "target": "One creature"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 corruption damage; I1 weakened (save ends)"
    "t2": "5 corruption damage; I2 weakened (save ends)"
    "t3": "6 corruption damage; I3 weakened (save ends) "
- "name": "Dizzying Hex"
  "type": "Maneuver"
  "cost": "1 Malice"
  "keywords":
  - "Magic"
  - "Ranged"
  - "Resistance"
  "distance": "Ranged 10"
  "target": "One creature"
  "effects":
  - "roll": "INU RR"
    "t1": "Prone and can't stand (save ends)"
    "t2": "Prone and can't stand (EoT)"
    "t3": "No effect "

```
