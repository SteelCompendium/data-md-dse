```ds-statblock
"name": "Dwarf Stonewhisperer"
"ancestry":
- "Dwarf"
- "Humanoid"
"roles":
- "Controller"
"level": !!int "3"
"ev": !!int "16"
"stamina": !!int "45"
"immunities": []
"weaknesses": []
"speed": "5"
"size": "1M"
"stability": !!int "2"
"free_strike": !!int "5"
"might": !!int "1"
"intuition": !!int "2"
"agility": !!int "0"
"reason": !!int "2"
"presence": !!int "0"
"traits":
- "name": "Stonewalker"
  "effect": "The stonewhisperer can phase through 2 squares of stone as part of any\
    \ movement they take. If they end their movement inside stone, they are shunted\
    \ out into the square where they entered it."
"abilities":
- "name": "Tile Slide"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Area"
  - "Magic"
  "distance": "3 cube within 1"
  "target": "All creatures and objects"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "3 damage; slide 1; M1 slowed (save ends)"
    "t2": "6 damage; slide 3; M2 slowed (save ends)"
    "t3": "9 damage; slide 5; M3 restrained (save ends)"
  - "name": "Effect"
    "effect": "A target restrained by a dwarf can be slid by this attack. "
- "name": "Stone Wave"
  "type": "Maneuver"
  "cost": "3 Malice"
  "keywords":
  - "Area"
  - "Ranged"
  "distance": "2 cube within 10"
  "target": "All enemies in the cube"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage; push 2; R1 slowed (save ends)"
    "t2": "3 damage; push 3; R2 slowed (save ends)"
    "t3": "4 damage; push 3; R3 slowed (save ends)"
  - "name": "Effect"
    "effect": "A target restrained by a dwarf can be pushed by this attack. The affected\
      \ area is difficult terrain for enemies. "

```
