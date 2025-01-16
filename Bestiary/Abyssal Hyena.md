```ds-statblock
"name": "Abyssal Hyena"
"ancestry":
- "Animal"
- "Gnoll"
"roles":
- "Brute"
- "Minion"
"level": !!int "2"
"ev": !!int "7"
"stamina": !!int "15"
"immunities": []
"weaknesses": []
"speed": "8"
"size": "1M"
"stability": !!int "1"
"free_strike": !!int "2"
"might": !!int "2"
"intuition": !!int "0"
"agility": !!int "1"
"reason": !!int "-3"
"presence": !!int "-2"
"traits":
- "name": "Death Snap"
  "effect": "When the abyssal hyena is reduced to 0 Stamina, they make a free strike\
    \ before dying."
"abilities":
- "name": "Snapjaw"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "Melee 1"
  "target": "1 creature or object per minion"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage"
    "t2": "4 damage; grabbed"
    "t3": "5 damage; grabbed "

```
