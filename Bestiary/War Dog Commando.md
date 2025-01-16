```ds-statblock
"name": "War Dog Commando"
"ancestry":
- "Humanoid"
- "War Dog"
"roles":
- "Ambusher"
- "Minion"
"level": !!int "1"
"ev": !!int "5"
"stamina": !!int "8"
"immunities": []
"weaknesses": []
"speed": "5"
"size": "1M"
"stability": !!int "0"
"free_strike": !!int "2"
"might": !!int "0"
"intuition": !!int "0"
"agility": !!int "2"
"reason": !!int "0"
"presence": !!int "0"
"traits":
- "name": "Loyalty Collar"
  "effect": "When the commando dies, they explode, dealing 1d6 damage to each adjacent\
    \ enemy."
"abilities":
- "name": "Daggers"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Ranged"
  - "Weapon"
  "distance": "Melee 1 or Ranged 5"
  "target": "One creature per minion"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage"
    "t2": "4 damage"
    "t3": "5 damage"
  - "name": "Effect"
    "effect": "The commando can use the Hide maneuver, even if observed. "

```
