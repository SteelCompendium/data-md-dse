```ds-statblock
"name": "Dwarf Hunter"
"ancestry":
- "Dwarf"
- "Humanoid"
"roles":
- "Support"
- "Minion"
"level": !!int "1"
"ev": !!int "6"
"stamina": !!int "12"
"immunities": []
"weaknesses": []
"speed": "5"
"size": "1M"
"stability": !!int "1"
"free_strike": !!int "2"
"might": !!int "1"
"intuition": !!int "0"
"agility": !!int "2"
"reason": !!int "0"
"presence": !!int "0"
"traits": []
"abilities":
- "name": "Snaring Javelin"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Ranged"
  - "Weapon"
  "distance": "Ranged 5"
  "target": "1 creature or object per minion"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage; pull 1"
    "t2": "4 damage; pull 2"
    "t3": "5 damage; pull 4"
  - "name": "Effect"
    "effect": "A target restrained by a dwarf can be pulled by this attack."

```
