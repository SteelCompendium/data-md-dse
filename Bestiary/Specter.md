```ds-statblock
"name": "Specter"
"ancestry":
- "Incorporeal"
- "Undead"
"roles":
- "Hexer"
"level": !!int "1"
"ev": !!int "7"
"stamina": !!int "12"
"immunities":
- "Corruption 3"
- "Poison 3"
"weaknesses": []
"speed": "5 (fly)"
"size": "1M"
"stability": !!int "1"
"free_strike": !!int "2"
"might": !!int "-5"
"intuition": !!int "0"
"agility": !!int "1"
"reason": !!int "0"
"presence": !!int "2"
"traits":
- "name": "Corruptive Phasing"
  "effect": "The specter can move through other creatures and objects at normal speed.\
    \ The first time in a round that the specter passes through a creature, that creature\
    \ takes 2 corruption damage."
"abilities":
- "name": "Decaying Touch"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Magic"
  - "Melee"
  "distance": "Melee 1"
  "target": "One creature"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 corruption damage; P1 weakened (save ends)"
    "t2": "4 corruption damage; P2 weakened (save ends)"
    "t3": "5 corruption damage; P3 weakened (save ends)"
  - "name": "2 Malice"
    "effect": "The potency of this ability increases by 1. A living creature killed\
      \ by this ability becomes a specter who appears in the target's space under\
      \ the Director's control. "
- "name": "Hidden Movement"
  "type": "Maneuver"
  "keywords":
  - "--"
  "distance": "Self"
  "target": "Self"
  "effects":
  - "name": "Effect"
    "effect": "The specter turns invisible, moves up to their speed, and becomes visible\
      \ again. "

```
