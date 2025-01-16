```ds-statblock
"name": "Wode Elf Greenskeeper"
"ancestry":
- "Fey"
- "Humanoid"
- "Wode Elf"
"roles":
- "Defender"
"level": !!int "1"
"ev": !!int "15"
"stamina": !!int "40"
"immunities": []
"weaknesses": []
"speed": "7"
"size": "1M"
"stability": !!int "0"
"free_strike": !!int "3"
"might": !!int "0"
"intuition": !!int "0"
"agility": !!int "2"
"reason": !!int "0"
"presence": !!int "1"
"traits":
- "name": "Masking Glamor"
  "effect": "The greenskeeper immediately hides at the end of their turn while in\
    \ cover or concealment, even if they are observed."
"abilities":
- "name": "Growing Longsword"
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
    "t1": "3 damage"
    "t2": "5 damage"
    "t3": "7 damage"
  - "name": "Effect"
    "effect": "Taunted (EoT). The greenskeeper can shift 3 after making the attack."
  - "name": "2 Malice"
    "effect": "The distance increases to Melee 5. "
- "name": "Overgrowth"
  "type": "Maneuver"
  "cost": "3 Malice"
  "keywords":
  - "Area"
  - "Ranged"
  "distance": "3 cube within 10"
  "target": "All enemies in the cube"
  "effects":
  - "name": "Effect"
    "effect": "The affected area is overgrown with heavy brush and bramble. It provides\
      \ cover and concealment for the greenskeeper and all allies, and is considered\
      \ difficult terrain for enemies. An enemy that starts their turn in an affected\
      \ square takes 3 damage. "

```
