```ds-statblock
"name": "Radenwight Swiftpaw"
"ancestry":
- "Humanoid"
- "Radenwight"
"roles":
- "Harrier"
- "Minion"
"level": !!int "1"
"ev": !!int "6"
"stamina": !!int "10"
"immunities": []
"weaknesses": []
"speed": "7 (climb)"
"size": "1S"
"stability": !!int "0"
"free_strike": !!int "2"
"might": !!int "0"
"intuition": !!int "0"
"agility": !!int "2"
"reason": !!int "1"
"presence": !!int "-1"
"traits": []
"abilities":
- "name": "Rapier Flunge"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "Melee 1"
  "target": "One creature or object per minion"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage; slide 1; the swiftpaw can shift 1 square"
    "t2": "4 damage; slide 2; the swiftpaw can shift 2 squares"
    "t3": "5 damage; slide 3; the swiftpaw can shift 3 squares "
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
    "effect": "The swiftpaw makes a free strike against the target."

```
