```ds-statblock
"name": "Lizardfolk Tonguer"
"ancestry":
- "Humanoid"
- "Lizardfolk"
"roles":
- "Artillery"
- "Minion"
"level": !!int "1"
"ev": !!int "6"
"stamina": !!int "8"
"immunities": []
"weaknesses": []
"speed": "5 (swim)"
"size": "1S"
"stability": !!int "0"
"free_strike": !!int "2"
"might": !!int "0"
"intuition": !!int "1"
"agility": !!int "2"
"reason": !!int "0"
"presence": !!int "0"
"traits":
- "name": "Reptilian Escape"
  "effect": "While the tonguer still has a tail, whenever the tonguer is grabbed,\
    \ slowed, weakened, or knocked prone, the tonguer can lose their tail to immediately\
    \ end the effect and shift 2."
"abilities":
- "name": "Tonguelash"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "Melee 8"
  "target": "1 creature or object per minion"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage; pull 1 or shift 1 towards target"
    "t2": "5 damage; pull 2 or shift 2 towards target"
    "t3": "6 damage; pull 3 or shift 3 towards target"
  - "name": "Effect"
    "effect": "If the target ends up in a space adjacent to the tonguer, they are\
      \ also grabbed. "

```
