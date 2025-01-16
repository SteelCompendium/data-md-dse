```ds-statblock
"name": "Dwarf Driver"
"ancestry":
- "Dwarf"
- "Humanoid"
"roles":
- "Harrier"
- "Minion"
"level": !!int "1"
"ev": !!int "6"
"stamina": !!int "12"
"immunities": []
"weaknesses": []
"speed": "7"
"size": "1M"
"stability": !!int "1"
"free_strike": !!int "2"
"might": !!int "2"
"intuition": !!int "0"
"agility": !!int "1"
"reason": !!int "0"
"presence": !!int "0"
"traits": []
"abilities":
- "name": "Handaxes"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Charge"
  - "Melee"
  - "Ranged"
  - "Weapon"
  "distance": "Melee 1 or Ranged 5"
  "target": "1 creature or object per minion"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage; push 1"
    "t2": "4 damage; push 2"
    "t3": "5 damage; push 4"
  - "name": "Effect"
    "effect": "A target restrained by a dwarf can be pushed by this attack."

```
