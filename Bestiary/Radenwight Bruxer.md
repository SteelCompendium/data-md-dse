```ds-statblock
"name": "Radenwight Bruxer"
"ancestry":
- "Humanoid"
- "Radenwight"
"roles":
- "Brute"
"level": !!int "1"
"ev": !!int "16"
"stamina": !!int "40"
"immunities": []
"weaknesses": []
"speed": "5 (climb)"
"size": "1M"
"stability": !!int "2"
"free_strike": !!int "5"
"might": !!int "2"
"intuition": !!int "0"
"agility": !!int "1"
"reason": !!int "-1"
"presence": !!int "0"
"traits":
- "name": "Lockdown"
  "effect": "An enemy can't shift while adjacent to the bruxer."
"abilities":
- "name": "Lockjaw"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "Melee 1"
  "target": "One creature or object"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "5 damage; M2 grabbed"
    "t2": "9 damage; M3 grabbed"
    "t3": "12 damage; grabbed"
  - "name": "Effect"
    "effect": "While the target is grabbed, they take 2 damage at the start of each\
      \ of the bruxer's turns. "
- "name": "Flurry of Bites"
  "type": "Action"
  "cost": "3 Malice"
  "keywords":
  - "Area"
  - "Weapon"
  "distance": "1 burst"
  "target": "All enemies in the burst"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "3 damage; A1 bleeding (save ends)"
    "t2": "5 damage; A2 bleeding (save ends)"
    "t3": "6 damage; A3 bleeding (save ends) "
- "name": "Ready Rodent"
  "type": "Triggered Action"
  "keywords":
  - "Melee"
  - "Weapon"
  "distance": "Melee 1"
  "target": "One creature"
  "trigger": "An ally deals damage to the target."
  "effects":
  - "name": "Effect"
    "effect": "The bruxer makes a free strike against the target. "

```
