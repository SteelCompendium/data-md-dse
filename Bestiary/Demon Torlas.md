```ds-statblock
"name": "Demon Torlas"
"ancestry":
- "Demon"
- "Planar"
"roles":
- "CONTROLLER"
"level": !!int "1"
"ev": !!int "9"
"stamina": !!int "15"
"immunities": []
"weaknesses":
- "Holy 3"
"speed": "5"
"size": "1S"
"stability": !!int "0"
"free_strike": !!int "2"
"might": !!int "0"
"intuition": !!int "0"
"agility": !!int "1"
"reason": !!int "0"
"presence": !!int "2"
"traits":
- "name": "Lethe"
  "effect": "While winded, the torlas has an edge on attacks, and attacks have an\
    \ edge against them."
- "name": "Soulsight"
  "effect": "Each creature within 2 of the torlas can't be hidden from them."
"abilities":
- "name": "Cronenstorm"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Area"
  - "Magic"
  - "Ranged"
  "distance": "3 cube within 10"
  "target": "Each creature in the cube"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "Slide 1"
    "t2": "Slide 2"
    "t3": "Slide 3"
  - "name": "Effect"
    "effect": "The area turns into a morass of spongy flesh before the targets are\
      \ force moved. Until the start of the torlas's next turn, the area is difficult\
      \ terrain, and each creature who moves within the area takes 1 damage for each\
      \ square moved. "
- "name": "Grasping Tendons"
  "type": "Maneuver"
  "keywords":
  - "Magic"
  - "Ranged"
  "distance": "Ranged 10"
  "target": "Three creatures"
  "effects":
  - "name": "Effect"
    "effect": "The torlas pulls each target 3 squares. "

```
