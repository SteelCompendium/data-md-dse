```ds-statblock
"name": "Goblin Stinker"
"ancestry":
- "Goblin"
- "Humanoid"
"roles":
- "Controller"
"level": !!int "1"
"ev": !!int "9"
"stamina": !!int "15"
"immunities": []
"weaknesses": []
"speed": "5 (climb)"
"size": "1S"
"stability": !!int "0"
"free_strike": !!int "2"
"might": !!int "-2"
"intuition": !!int "0"
"agility": !!int "1"
"reason": !!int "0"
"presence": !!int "2"
"traits":
- "name": "Crafty"
  "effect": "The stinker doesn't provoke opportunity attacks by moving."
"abilities":
- "name": "Toxic Winds"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Area"
  - "Magic"
  - "Ranged"
  "distance": "3 cube within 10"
  "target": "Each enemy"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "1 poison damage; slide 1"
    "t2": "2 poison damage; slide 2"
    "t3": "3 poison damage; slide 3"
  - "name": "1 Malice"
    "effect": "Increase the slide for one target by 2 squares. "
- "name": "Swamp Gas"
  "type": "Maneuver"
  "keywords":
  - "Area"
  - "Magic"
  - "Ranged"
  "distance": "3 cube within 10"
  "target": "Special"
  "effects":
  - "name": "Effect"
    "effect": "The area is filled with a green haze until the start of the stinker's\
      \ next turn or until the stinker is reduced to Stamina 0. The area is difficult\
      \ terrain for non-goblin creatures, and each such creature who moves within\
      \ the area takes 2 poison damage for each square moved. The haze can't be dispersed\
      \ by wind. "

```
