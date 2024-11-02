```ds-statblock
"name": "Goblin Spinecleaver"
"ancestry":
- "Goblin"
- "Humanoid"
"roles":
- "Brute"
- "Minion"
"level": !!int "1"
"ev": !!int "6"
"stamina": !!int "10"
"immunities": []
"weaknesses": []
"speed": "5 (climb)"
"size": "1S"
"stability": !!int "0"
"free_strike": !!int "2"
"might": !!int "2"
"intuition": !!int "0"
"agility": !!int "0"
"reason": !!int "0"
"presence": !!int "-1"
"traits":
- "name": "Crafty"
  "effect": "The spinecleaver doesn't provoke opportunity attacks by moving."
"abilities":
- "name": "Axe"
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
    "t1": "2 damage; push 1"
    "t2": "4 damage; push 3"
    "t3": "5 damage; push 4 "

```
