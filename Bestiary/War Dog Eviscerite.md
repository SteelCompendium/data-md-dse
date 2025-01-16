```ds-statblock
"name": "War Dog Eviscerite"
"ancestry":
- "Humanoid"
- "War Dog"
"roles":
- "Harrier"
"level": !!int "1"
"ev": !!int "10"
"stamina": !!int "20"
"immunities": []
"weaknesses": []
"speed": "7"
"size": "1M"
"stability": !!int "0"
"free_strike": !!int "3"
"might": !!int "1"
"intuition": !!int "0"
"agility": !!int "2"
"reason": !!int "0"
"presence": !!int "0"
"traits":
- "name": "Loyalty Collar"
  "effect": "When the eviscerite dies, they explode, dealing 1d6 damage to each adjacent\
    \ enemy."
"abilities":
- "name": "Chainsaw Whip"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "Melee 3"
  "target": "One creature or object"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "3 damage"
    "t2": "5 damage; pull 1"
    "t3": "7 damage; pull 2"
  - "name": "Effect"
    "effect": "The eviscerite can grab a target pulled adjacent to them by this ability. "
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
