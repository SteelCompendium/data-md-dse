```ds-statblock
"name": "Goblin Sniper"
"ancestry":
- "Goblin"
- "Humanoid"
"roles":
- "Artillery"
- "Minion"
"level": !!int "1"
"ev": !!int "4"
"stamina": !!int "5"
"immunities": []
"weaknesses": []
"speed": "5 (climb)"
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
  "effect": "The sniper doesn't provoke opportunity attacks by moving."
"abilities":
- "name": "Bow"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Ranged"
  - "Weapon"
  "distance": "Ranged 10"
  "target": "One creature or object per minion"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage"
    "t2": "4 damage"
    "t3": "5 damage"
  - "name": "Effect"
    "effect": "If the sniper doesn't use a maneuver or a move action this turn, the\
      \ ability has edge. "

```
