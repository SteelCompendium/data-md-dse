```ds-statblock
"name": "Lizardfolk Shellguard"
"ancestry":
- "Humanoid"
- "Lizardfolk"
"roles":
- "Defender"
- "Minion"
"level": !!int "1"
"ev": !!int "7"
"stamina": !!int "12"
"immunities": []
"weaknesses": []
"speed": "5 (swim)"
"size": "1L"
"stability": !!int "1"
"free_strike": !!int "2"
"might": !!int "2"
"intuition": !!int "0"
"agility": !!int "1"
"reason": !!int "0"
"presence": !!int "0"
"traits":
- "name": "Reptilian Escape"
  "effect": "While the shellguard still has a tail, whenever the shellguard is grabbed,\
    \ slowed, weakened, or knocked prone, the shellguard can lose their tail to immediately\
    \ end the effect and shift 2."
"abilities":
- "name": "Shield Smash"
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
    "t2": "4 damage"
    "t3": "5 damage"
  - "name": "Effect"
    "effect": "All allies have **advantage** against the target's next attack. "

```
