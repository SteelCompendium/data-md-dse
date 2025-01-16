```ds-statblock
"name": "Wight"
"ancestry":
- "Corporeal"
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
"speed": "5"
"size": "1M"
"stability": !!int "0"
"free_strike": !!int "2"
"might": !!int "2"
"intuition": !!int "0"
"agility": !!int "1"
"reason": !!int "0"
"presence": !!int "1"
"traits":
- "name": "Arise"
  "effect": "The first time the wight is reduced to Stamina 0 by damage that isn't\
    \ fire damage or holy damage and their body isn't destroyed, they regain half\
    \ their Stamina and fall prone."
"abilities":
- "name": "Lifestealer Longsword"
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
    "t1": "2 corruption damage"
    "t2": "4 corruption damage; M1 slowed (save ends)"
    "t3": "5 corruption damage; M2 slowed and weakened (save ends)"
  - "name": "Effect"
    "effect": "The target appears to rapidly age each time they take damage from this\
      \ attack. The target regains their former appearance when the wight is destroyed. "
- "name": "Raise"
  "type": "Maneuver"
  "cost": "3 Malice"
  "keywords":
  - "Magic"
  - "Ranged"
  "distance": "Ranged 3"
  "target": "One dead ally"
  "effects":
  - "name": "Effect"
    "effect": "The target revives with half their Stamina. The wight can't use this\
      \ maneuver again until they attack a creature with their lifestealer longsword. "

```
