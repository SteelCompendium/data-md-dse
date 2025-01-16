```ds-statblock
"name": "Lizardfolk Grunt"
"ancestry":
- "Humanoid"
- "Lizardfolk"
"roles":
- "Harrier"
- "Minion"
"level": !!int "1"
"ev": !!int "6"
"stamina": !!int "10"
"immunities": []
"weaknesses": []
"speed": "6 (swim)"
"size": "1M"
"stability": !!int "0"
"free_strike": !!int "2"
"might": !!int "1"
"intuition": !!int "0"
"agility": !!int "2"
"reason": !!int "0"
"presence": !!int "0"
"traits":
- "name": "Reptilian Escape"
  "effect": "While the grunt still has a tail, whenever the grunt is grabbed, slowed,\
    \ weakened, or knocked prone, the grunt can lose their tail to immediately end\
    \ the effect and shift 2."
"abilities":
- "name": "Snap and Toss"
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
    "t2": "4 damage; slide 2"
    "t3": "5 damage; slide 4 "

```
