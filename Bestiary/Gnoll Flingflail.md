```ds-statblock
"name": "Gnoll Flingflail"
"ancestry":
- "Fiend"
- "Gnoll"
"roles":
- "Artillery"
- "Minion"
"level": !!int "2"
"ev": !!int "5"
"stamina": !!int "8"
"immunities": []
"weaknesses": []
"speed": "5"
"size": "1M"
"stability": !!int "1"
"free_strike": !!int "2"
"might": !!int "2"
"intuition": !!int "0"
"agility": !!int "0"
"reason": !!int "1"
"presence": !!int "-2"
"traits":
- "name": "Death Frenzy"
  "effect": "Whenever an ally within 5 is reduced to 0 Stamina, the flingflail archer\
    \ moves up to their speed and makes a free strike."
"abilities":
- "name": "Chain Shotput"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Ranged"
  - "Weapon"
  "distance": "Ranged 8"
  "target": "1 creature or object per minion"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage"
    "t2": "4 damage; push 1"
    "t3": "5 damage; push 3 "

```
