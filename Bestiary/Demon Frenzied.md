```ds-statblock
"name": "Demon Frenzied"
"ancestry":
- "Demon"
- "Planar"
"roles":
- "HARRIER"
- "MINION"
"level": !!int "1"
"ev": !!int "4"
"stamina": !!int "8"
"immunities": []
"weaknesses":
- "Holy 3"
"speed": "6"
"size": "1M"
"stability": !!int "0"
"free_strike": !!int "2"
"might": !!int "0"
"intuition": !!int "-1"
"agility": !!int "2"
"reason": !!int "-1"
"presence": !!int "-1"
"traits":
- "name": "Soulsight"
  "effect": "Each creature within 2 of the frenzied can't be hidden from them."
"abilities":
- "name": "Rip and Tear"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Charge"
  - "Melee"
  - "Weapon"
  "distance": "Melee 1"
  "target": "One creature or object per minion"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage"
    "t2": "3 damage"
    "t3": "4 damage "

```
