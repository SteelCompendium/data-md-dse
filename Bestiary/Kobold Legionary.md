```ds-statblock
"name": "Kobold Legionary"
"ancestry":
- "Humanoid"
- "Kobold"
"roles":
- "Defender"
"level": !!int "1"
"ev": !!int "9"
"stamina": !!int "20"
"immunities": []
"weaknesses": []
"speed": "5"
"size": "1S"
"stability": !!int "0"
"free_strike": !!int "1"
"might": !!int "2"
"intuition": !!int "0"
"agility": !!int "1"
"reason": !!int "0"
"presence": !!int "0"
"traits":
- "name": "Shield? Shield!"
  "effect": "The legionary has increased Stability by 1 and can act as cover for allies\
    \ when adjacent to an ally who also has this trait."
"abilities":
- "name": "Gladius"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "Melee 1"
  "target": "1 creature or object"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage"
    "t2": "4 damage"
    "t3": "5 damage"
  - "name": "Effect"
    "effect": "Taunted (EoT)."
  - "name": "3 Malice"
    "effect": "The legionary and their squad can shift 2 before this attack is made. "
- "name": "Shield Bash"
  "type": "Maneuver"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "Melee 1"
  "target": "1 creature or object"
  "t1": "1 damage; push 1; 1 prone"
  "t2": "2 damage; push 2; 2 prone"
  "t3": "3 damage; push 3; 3 prone "

```
