```ds-statblock
"name": "Demon Muceron"
"ancestry":
- "Demon"
- "Planar"
"roles":
- "BRUTE"
"level": !!int "3"
"ev": !!int "18"
"stamina": !!int "45"
"immunities": []
"weaknesses":
- "Holy 3"
"speed": "5"
"size": "1M"
"stability": !!int "0"
"free_strike": !!int "5"
"might": !!int "2"
"intuition": !!int "0"
"agility": !!int "2"
"reason": !!int "0"
"presence": !!int "1"
"traits":
- "name": "Lethe"
  "effect": "While winded, the muceron has an edge on attacks, and attacks have an\
    \ edge against them."
- "name": "Soulsight"
  "effect": "Each creature within 2 of the muceron can't be hidden from them."
"abilities":
- "name": "Barbed Tongues"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "Melee 2"
  "target": "One creature"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "5 damage; pull 2"
    "t2": "8 damage; pull 3"
    "t3": "11 damage; pull 4"
  - "name": "Effect"
    "effect": "Taunted (EoT). "
- "name": "Tongue Pull"
  "type": "Maneuver"
  "cost": "2 Malice"
  "keywords":
  - "Attack"
  - "Ranged"
  - "Weapon"
  "distance": "Ranged 5"
  "target": "Three creatures"
  "effects":
  - "name": "Effect"
    "effect": "The muceron pulls each target 5 squares. "

```
