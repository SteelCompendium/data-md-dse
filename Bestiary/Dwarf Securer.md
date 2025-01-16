```ds-statblock
"name": "Dwarf Securer"
"ancestry":
- "Dwarf"
- "Humanoid"
"roles":
- "Brute"
- "Minion"
"level": !!int "1"
"ev": !!int "8"
"stamina": !!int "14"
"immunities": []
"weaknesses": []
"speed": "5"
"size": "1M"
"stability": !!int "2"
"free_strike": !!int "2"
"might": !!int "2"
"intuition": !!int "0"
"agility": !!int "0"
"reason": !!int "0"
"presence": !!int "0"
"traits": []
"abilities":
- "name": "Maul"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Charge"
  - "Melee"
  - "Weapon"
  "distance": "Melee 1"
  "target": "1 creature or object per minion"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage"
    "t2": "5 damage; grabbed"
    "t3": "6 damage; grabbed or prone"

```
