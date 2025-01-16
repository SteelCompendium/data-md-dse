```ds-statblock
"name": "Demon Remasch"
"ancestry":
- "Demon"
- "Planar"
"roles":
- "AMBUSHER"
"level": !!int "2"
"ev": !!int "13"
"stamina": !!int "25"
"immunities": []
"weaknesses":
- "Holy 3"
"speed": "5 (teleport)"
"size": "1S"
"stability": !!int "0"
"free_strike": !!int "4"
"might": !!int "0"
"intuition": !!int "0"
"agility": !!int "2"
"reason": !!int "0"
"presence": !!int "2"
"traits":
- "name": "Lethe"
  "effect": "While winded, the remasch has an edge on attacks, and attacks have an\
    \ edge against them."
- "name": "Soulsight"
  "effect": "Each creature within 2 of the remasch can't be hidden from them."
"abilities":
- "name": "Abyssal Strike"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "Melee 1"
  "target": "One creature or object"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "4 damage; the remasch teleports 2 squares"
    "t2": "7 damage; the remasch teleports 3 squares"
    "t3": "10 damage; the remasch teleports 5 squares"
  - "name": "5 Malice"
    "effect": "The remasch takes an adjacent creature with them when they teleport.\
      \ The creature appears in an unoccupied space adjacent to the remasch's destination. "
- "name": "Grasping Shadow"
  "type": "Maneuver"
  "cost": "3 Malice"
  "keywords":
  - "Magic"
  "distance": "Self"
  "target": "Self"
  "effects":
  - "name": "Effect"
    "effect": "The remasch teleports 2 squares and uses Abyssal Strike. "

```
