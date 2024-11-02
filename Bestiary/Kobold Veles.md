```ds-statblock
"name": "Kobold Veles"
"ancestry":
- "Humanoid"
- "Kobold"
"roles":
- "Harrier"
- "Minion"
"level": !!int "1"
"ev": !!int "3"
"stamina": !!int "5"
"immunities": []
"weaknesses": []
"speed": "6"
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
  "effect": "The veles has increased Stability by 1 and can act as cover for allies\
    \ when adjacent to an ally who also has this trait."
"abilities":
- "name": "Pilum"
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
    "t1": "1 damage"
    "t2": "2 damage"
    "t3": "3 damage"
  - "name": "Effect"
    "effect": "All kobolds ignore opportunity attacks from the target until the start\
      \ of the veles' next turn. "

```
