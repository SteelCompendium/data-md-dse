```ds-statblock
"name": "War Dog Conscript"
"ancestry":
- "Humanoid"
- "War Dog"
"roles":
- "Harrier"
- "Minion"
"level": !!int "1"
"ev": !!int "4"
"stamina": !!int "8"
"immunities": []
"weaknesses": []
"speed": "7"
"size": "1M"
"stability": !!int "0"
"free_strike": !!int "2"
"might": !!int "2"
"intuition": !!int "0"
"agility": !!int "0"
"reason": !!int "0"
"presence": !!int "0"
"traits":
- "name": "Loyalty Collar"
  "effect": "When the conscript dies, they explode, dealing 1d6 damage to each adjacent\
    \ enemy."
"abilities":
- "name": "Blade"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Charge"
  - "Melee"
  - "Ranged"
  - "Weapon"
  "distance": "Melee 1 or Ranged 5"
  "target": "One creature per minion"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage"
    "t2": "3 damage"
    "t3": "4 damage"
  - "name": "Effect"
    "effect": "If this ability is used as part of the Charge action, the conscript\
      \ has **edge** on the attack. "

```
