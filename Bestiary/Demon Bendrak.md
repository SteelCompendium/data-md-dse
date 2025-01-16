```ds-statblock
"name": "Demon Bendrak"
"ancestry":
- "Demon"
- "Planar"
"roles":
- "HEXER"
"level": !!int "2"
"ev": !!int "11"
"stamina": !!int "20"
"immunities": []
"weaknesses":
- "Holy 3"
"speed": "5"
"size": "1S"
"stability": !!int "0"
"free_strike": !!int "3"
"might": !!int "0"
"intuition": !!int "0"
"agility": !!int "1"
"reason": !!int "0"
"presence": !!int "2"
"traits":
- "name": "Lethe"
  "effect": "While winded, the bendrak has an edge on attacks, and attacks have an\
    \ edge against them."
- "name": "Soulsight"
  "effect": "Each creature within 2 of the bendrak can't be hidden from them."
"abilities":
- "name": "Warp Perceptions"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Magic"
  - "Ranged"
  "distance": "Ranged 10"
  "target": "One creature"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "3 psychic damage; P1 weakened (save ends)"
    "t2": "5 psychic damage; P2 weakened (save ends)"
    "t3": "7 psychic damage; P3 weakened (save ends)"
  - "name": "Effect"
    "effect": "If the target makes an attack while weakened this way, the bendrak\
      \ can choose a second target for the attack within the distance of the attack,\
      \ then evenly divides any damage from the attack between the two targets. "
- "name": "Vanish"
  "type": "Maneuver"
  "cost": "1 Malice"
  "keywords":
  - "Magic"
  - "Ranged"
  "distance": "Ranged 10"
  "target": "Self or one ally"
  "effects":
  - "name": "Effect"
    "effect": "The target immediately becomes hidden, regardless of whether they have\
      \ cover or concealment. "

```
