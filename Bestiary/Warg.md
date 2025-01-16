```ds-statblock
"name": "Warg"
"ancestry":
- "Animal"
- "Goblin"
"roles":
- "Mount"
"level": !!int "1"
"ev": !!int "10"
"stamina": !!int "20"
"immunities": []
"weaknesses": []
"speed": "7"
"size": "1L"
"stability": !!int "1"
"free_strike": !!int "2"
"might": !!int "1"
"intuition": !!int "0"
"agility": !!int "2"
"reason": !!int "-1"
"presence": !!int "-1"
"traits":
- "name": "Mounted Charger"
  "effect": "If a warg used as a mount charges, their rider gains an edge on melee\
    \ attacks until the end of their turn."
- "name": "Shared Crafty"
  "effect": "If the warg's rider has the Crafty trait, the warg also has the Crafty\
    \ trait."
"abilities":
- "name": "Bite"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Charge"
  - "Melee"
  - "Weapon"
  "distance": "Melee 1"
  "target": "One creature or object"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage"
    "t2": "5 damage"
    "t3": "6 damage "
- "name": "Sprint"
  "type": "Maneuver"
  "cost": "1 Malice"
  "keywords":
  - "--"
  "distance": "Self"
  "target": "Self"
  "effects":
  - "name": "Effect"
    "effect": "The warg moves up to their speed. "

```
