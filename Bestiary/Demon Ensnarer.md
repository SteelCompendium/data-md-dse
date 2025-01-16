```ds-statblock
"name": "Demon Ensnarer"
"ancestry":
- "Demon"
- "Planar"
"roles":
- "BRUTE"
- "MINION"
"level": !!int "1"
"ev": !!int "6"
"stamina": !!int "10"
"immunities": []
"weaknesses":
- "Holy 3"
"speed": "5"
"size": "1M"
"stability": !!int "0"
"free_strike": !!int "2"
"might": !!int "2"
"intuition": !!int "-1"
"agility": !!int "0"
"reason": !!int "-1"
"presence": !!int "-1"
"traits":
- "name": "Soulsight"
  "effect": "Each creature within 2 of the ensnarer can't be hidden from them."
"abilities":
- "name": "Barbed Tongues"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "Melee 3"
  "target": "One creature or object per minion"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage; pull 1"
    "t2": "4 damage; pull 2"
    "t3": "5 damage; pull 3"
  - "name": "Effect"
    "effect": "If the target is pulled adjacent to the ensnarer, the ensnarer takes\
      \ a free strike against them. "

```
