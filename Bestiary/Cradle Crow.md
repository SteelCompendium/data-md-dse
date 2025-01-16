```ds-statblock
"name": "Cradle Crow"
"ancestry":
- "Construct"
- "High Elf"
"roles":
- "Harrier"
- "Minion"
"level": !!int "1"
"ev": !!int "6"
"stamina": !!int "10"
"immunities": []
"weaknesses": []
"speed": "7 (fly)"
"size": "1T"
"stability": !!int "0"
"free_strike": !!int "2"
"might": !!int "0"
"intuition": !!int "0"
"agility": !!int "2"
"reason": !!int "0"
"presence": !!int "1"
"traits": []
"abilities":
- "name": "Heckle"
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
    "t2": "4 damage; taunted (EoT)"
    "t3": "5 damage; taunted (EoT)"
  - "name": "Effect"
    "effect": "The cradle crow ignores opportunity attacks from the target until the\
      \ end of its turn."

```
