```ds-statblock
"name": "Skitterling"
"ancestry":
- "Animal"
- "Goblin"
"roles":
- "Hexer"
- "Minion"
"level": !!int "1"
"ev": !!int "3"
"stamina": !!int "5"
"immunities": []
"weaknesses": []
"speed": "5 (fly)"
"size": "1T"
"stability": !!int "0"
"free_strike": !!int "2"
"might": !!int "-5"
"intuition": !!int "0"
"agility": !!int "2"
"reason": !!int "-4"
"presence": !!int "-2"
"traits": []
"abilities":
- "name": "Claws"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "Melee 1"
  "target": "One creature or object per minion"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 poison damage"
    "t2": "3 poison damage"
    "t3": "4 poison damage"
  - "name": "Effect"
    "effect": "The target has a bane on their next attack."

```
