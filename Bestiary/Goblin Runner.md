```ds-statblock
"name": "Goblin Runner"
"ancestry":
- "Goblin"
- "Humanoid"
"roles":
- "Harrier"
- "Minion"
"level": !!int "1"
"ev": !!int "4"
"stamina": !!int "8"
"immunities": []
"weaknesses": []
"speed": "6 (climb)"
"size": "1S"
"stability": !!int "0"
"free_strike": !!int "2"
"might": !!int "-2"
"intuition": !!int "0"
"agility": !!int "2"
"reason": !!int "0"
"presence": !!int "-1"
"traits":
- "name": "Crafty"
  "effect": "The runner doesn't provoke opportunity attacks by moving."
"abilities":
- "name": "Club"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Charge"
  - "Melee"
  - "Weapon"
  "distance": "Melee 1"
  "target": "One creature or object per minion"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage"
    "t2": "3 damage"
    "t3": "4 damage "

```
