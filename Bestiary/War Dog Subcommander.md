```ds-statblock
"name": "War Dog Subcommander"
"ancestry":
- "Humanoid"
- "War Dog"
"roles":
- "Support"
"level": !!int "2"
"ev": !!int "12"
"stamina": !!int "25"
"immunities": []
"weaknesses": []
"speed": "5"
"size": "1M"
"stability": !!int "0"
"free_strike": !!int "3"
"might": !!int "2"
"intuition": !!int "0"
"agility": !!int "0"
"reason": !!int "0"
"presence": !!int "1"
"traits":
- "name": "The Iron Saint Does Not Recognize Retreat"
  "effect": "Each ally within 5 squares of the subcommander adds 3 to their stability."
- "name": "Loyalty Collar"
  "effect": "When the subcommander dies, they explode, dealing 1d6 damage to each\
    \ adjacent enemy."
"abilities":
- "name": "Command Saber"
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
    "t1": "3 damage"
    "t2": "5 damage"
    "t3": "7 damage"
  - "name": "Effect"
    "effect": "An ally within 5 squares of the subcommander can make a free strike\
      \ against the target. "
- "name": "Posthumous Promotion"
  "type": "Maneuver"
  "keywords":
  - "Magic"
  - "Ranged"
  "distance": "Ranged 10"
  "target": "One war dog with a loyalty collar"
  "effects":
  - "name": "Effect"
    "effect": "The target's loyalty collar detonates, killing them instantly. "

```
