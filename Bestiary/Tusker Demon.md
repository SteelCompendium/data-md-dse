```ds-statblock
"name": "Tusker Demon"
"ancestry":
- "Demon"
- "Gnoll"
- "Planar"
"roles":
- "Brute"
"level": !!int "2"
"ev": !!int "15"
"stamina": !!int "35"
"immunities":
- "weapon 3"
"weaknesses": []
"speed": "7"
"size": "3"
"stability": !!int "3"
"free_strike": !!int "4"
"might": !!int "2"
"intuition": !!int "0"
"agility": !!int "-1"
"reason": !!int "-3"
"presence": !!int "-1"
"traits":
- "name": "Trample"
  "effect": "The tusker demon can move through enemies and objects at normal speed.\
    \ When the tusker enters a creature's space for the first time on their turn,\
    \ the creature takes 2d6 damage. The tusker demon can end their turn in a prone\
    \ size 1 creature's space, preventing the creature from getting up."
- "name": "Lethe"
  "effect": "While winded, the tusker demon has edge on attacks, and attacks have\
    \ edge against them."
"abilities":
- "name": "Gore"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Charge"
  - "Melee"
  - "Weapon"
  "distance": "Melee 2"
  "target": "1 creature or object"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "4 damage; push 1"
    "t2": "7 damage; push 2"
    "t3": "10 damage; push 3; prone"
  - "name": "Effect"
    "effect": "This attack has edge while charging. "
- "name": "Vengeful Tusker"
  "type": "Triggered Action"
  "keywords":
  - "--"
  "trigger": "An enemy within 7 deals damage to the tusker."
  "distance": "Self"
  "target": "Self"
  "effects":
  - "name": "Effect"
    "effect": "The tusker demon charges the target using Gore. "

```
