```ds-statblock
"name": "Trained Gelatinous Cube"
"ancestry":
- "Animal"
- "Kobold"
"roles":
- "Hexer"
"level": !!int "1"
"ev": !!int "16"
"stamina": !!int "20"
"immunities":
- "Acid 3"
- "Weapon 3"
"weaknesses": []
"speed": "5"
"size": "2"
"stability": !!int "2"
"free_strike": !!int "4"
"might": !!int "2"
"intuition": !!int "0"
"agility": !!int "-1"
"reason": !!int "-3"
"presence": !!int "-2"
"traits":
- "name": "Translucent Cube"
  "effect": "The cube completely occupies its space, blocking line of effect on enemy\
    \ attacks and abilities. The cube is hidden until revealed."
"abilities":
- "name": "Engulf"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "Melee 1"
  "target": "1 creature or object"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "3 acid damage; 1 dazed (save ends)"
    "t2": "5 acid damage; 2 dazed (save ends)"
    "t3": "7 acid damage; 3 restrained (save ends)"
  - "name": "Effect"
    "effect": "A size 2 or smaller creature restrained by this attack is pulled into\
      \ one of the cube's squares and moves with the cube. The creature takes 3 acid\
      \ damage at the start of each of their turns while restrained. When restrained\
      \ ends, the creature moves to the nearest unoccupied square adjacent to the\
      \ cube."
  - "name": "3 Malice"
    "effect": "The cube attacks 1 additional target. "
- "name": "You Didn't Pay Attention!"
  "type": "Free Triggered Action"
  "keywords":
  - "--"
  "trigger": "A creature moves or is force moved into the cube."
  "distance": "Self"
  "target": "Self"
  "effects":
  - "name": "Effect"
    "effect": "The cube uses Engulf with a double edge. "

```
