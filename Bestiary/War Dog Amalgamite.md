```ds-statblock
"name": "War Dog Amalgamite"
"ancestry":
- "Humanoid"
- "War Dog"
"roles":
- "Brute"
"level": !!int "2"
"ev": !!int "15"
"stamina": !!int "35"
"immunities": []
"weaknesses": []
"speed": "5"
"size": "2"
"stability": !!int "2"
"free_strike": !!int "4"
"might": !!int "2"
"intuition": !!int "0"
"agility": !!int "0"
"reason": !!int "0"
"presence": !!int "0"
"traits":
- "name": "Loyalty Collar"
  "effect": "When the amalgamite dies, they explode, dealing 1d6 damage to each adjacent\
    \ enemy."
"abilities":
- "name": "Several Arms"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "Melee 2"
  "target": "Two creatures or objects"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "3 damage; A1 grabbed"
    "t2": "4 damage; A2 grabbed"
    "t3": "5 damage; A3 grabbed"
  - "name": "Special"
    "effect": "The amalgamite can grab up to four creatures."
  - "name": "5 Malice"
    "effect": "The amalgamite deals an additional 4 damage to each creature they have\
      \ grabbed and regains Stamina equal to the damage dealt. "
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
