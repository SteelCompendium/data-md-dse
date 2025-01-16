```ds-statblock
"name": "Lizardfolk Scaletooth"
"ancestry":
- "Humanoid"
- "Lizardfolk"
"roles":
- "Brute"
"level": !!int "1"
"ev": !!int "16"
"stamina": !!int "40"
"immunities":
- "weapon 3"
"weaknesses": []
"speed": "5 (swim)"
"size": "1M"
"stability": !!int "0"
"free_strike": !!int "5"
"might": !!int "2"
"intuition": !!int "0"
"agility": !!int "1"
"reason": !!int "0"
"presence": !!int "0"
"traits":
- "name": "Reptilian Escape"
  "effect": "While the scaletooth still has a tail, whenever the scaletooth is grabbed,\
    \ slowed, weakened, or knocked prone, the scaletooth can lose their tail to immediately\
    \ end the effect and shift 2."
"abilities":
- "name": "Razor Bite"
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
    "t1": "5 damage; A1 bleeding (save ends)"
    "t2": "9 damage; A2 bleeding (save ends)"
    "t3": "12 damage; A3 bleeding (save ends)"
  - "name": "Effect"
    "effect": "The potency of this attack increases by 1 if the target is grabbed\
      \ by the scaletooth. "
- "name": "Tail Whip"
  "type": "Action"
  "cost": "2 Malice"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "Melee 2"
  "target": "2 creatures or objects"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "3 damage; slide 1; M1 grappled"
    "t2": "5 damage; slide 2; M2 grappled"
    "t3": "6 damage; slide 3; M3 grappled if within 2 of the scaletooth"
  - "name": "Effect"
    "effect": "The scaletooth needs their tail to use this ability. The scaletooth\
      \ can't grapple more than one creature or object with this ability. "

```
