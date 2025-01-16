```ds-statblock
"name": "Dwarf Lurer"
"ancestry":
- "Dwarf"
- "Humanoid"
"roles":
- "Defender"
- "Minion"
"level": !!int "1"
"ev": !!int "7"
"stamina": !!int "14"
"immunities": []
"weaknesses": []
"speed": "5"
"size": "1M"
"stability": !!int "2"
"free_strike": !!int "2"
"might": !!int "1"
"intuition": !!int "2"
"agility": !!int "0"
"reason": !!int "0"
"presence": !!int "0"
"traits": []
"abilities":
- "name": "Whistling Axes"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Ranged"
  - "Weapon"
  "distance": "Melee 1 or Ranged 5"
  "target": "1 creature or object per minion"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage"
    "t2": "4 damage"
    "t3": "5 damage; an ally adjacent to the target can make a free strike"
  - "name": "Effect"
    "effect": "The target can't use triggered actions until the start of the next\
      \ round."

```
