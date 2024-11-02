```ds-statblock
"name": "Kobold Tiro"
"ancestry":
- "Humanoid"
- "Kobold"
"roles":
- "Defender"
- "Minion"
"level": !!int "1"
"ev": !!int "3"
"stamina": !!int "8"
"immunities": []
"weaknesses": []
"speed": "5"
"size": "1S"
"stability": !!int "0"
"free_strike": !!int "1"
"might": !!int "0"
"intuition": !!int "0"
"agility": !!int "2"
"reason": !!int "0"
"presence": !!int "0"
"traits":
- "name": "Shield? Shield!"
  "effect": "The tiro has increased Stability by 1 and can act as cover for allies\
    \ when adjacent to an ally who also has this trait."
"abilities":
- "name": "Pugio"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "Melee 2"
  "target": "1 creature or object per minion"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "1 damage"
    "t2": "2 damage; shift 1"
    "t3": "3 damage; shift 2 "

```
