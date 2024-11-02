```ds-statblock
"name": "Crawling Claw"
"ancestry":
- "Corporeal"
- "Undead"
"roles":
- "Harrier"
- "Minion"
"level": !!int "1"
"ev": !!int "2"
"stamina": !!int "5"
"immunities":
- "Corruption 2"
- "Poison 2"
"weaknesses": []
"speed": "6 (climb)"
"size": "1T"
"stability": !!int "0"
"free_strike": !!int "1"
"might": !!int "0"
"intuition": !!int "-1"
"agility": !!int "2"
"reason": !!int "-5"
"presence": !!int "-1"
"traits":
- "name": "Disorganized"
  "effect": "The crawling claw can't grant the flanking benefit to allies."
"abilities":
- "name": "Fingernails"
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
    "t1": "1 damage"
    "t2": "2 damage"
    "t3": "3 damage"
  - "name": "Effect"
    "effect": "The crawling claw shifts a number of squares equal to the damage dealt. "

```
