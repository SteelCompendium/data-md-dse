```ds-statblock
"name": "Kobold Artifex"
"ancestry":
- "Humanoid"
- "Kobold"
"roles":
- "Controller"
"level": !!int "1"
"ev": !!int "7"
"stamina": !!int "12"
"immunities": []
"weaknesses": []
"speed": "5"
"size": "1S"
"stability": !!int "0"
"free_strike": !!int "1"
"might": !!int "0"
"intuition": !!int "0"
"agility": !!int "2"
"reason": !!int "1"
"presence": !!int "0"
"traits":
- "name": "Shield? Shield!"
  "effect": "The artifex has increased Stability by 1 and can act as cover for allies\
    \ when adjacent to an ally who also has this trait."
"abilities":
- "name": "Chain Hook"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Ranged"
  - "Weapon"
  "distance": "Ranged 5"
  "target": "1 creature or object"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage; pull 1"
    "t2": "4 damage; pull 2"
    "t3": "5 damage; pull 3"
  - "name": "Effect"
    "effect": "If the target's forced movement triggers a trap, the target has a bane\
      \ on all resistance rolls against that trap. "
- "name": "Activate Trap"
  "type": "Maneuver"
  "keywords":
  - "--"
  "distance": "Ranged 10"
  "target": "1 trap or terrain object"
  "effects":
  - "name": "Effect"
    "effect": "The trap or terrain object instantly triggers."
  - "name": "3 Malice"
    "effect": "The artifex can place a new trap in the encounter and instantly trigger\
      \ it. "

```
