```ds-statblock
"name": "Ghoul"
"ancestry":
- "Corporeal"
- "Undead"
"roles":
- "Harrier"
"level": !!int "1"
"ev": !!int "8"
"stamina": !!int "15"
"immunities":
- "Corruption 3"
- "Poison 3"
"weaknesses": []
"speed": "7"
"size": "1M"
"stability": !!int "0"
"free_strike": !!int "3"
"might": !!int "0"
"intuition": !!int "0"
"agility": !!int "2"
"reason": !!int "-2"
"presence": !!int "-1"
"traits":
- "name": "Hunger"
  "effect": "If the ghoul charges, their speed increases by 2 until the end of their\
    \ turn."
- "name": "Arise"
  "effect": "The first time the ghoul is reduced to Stamina 0 by damage that isn't\
    \ fire damage or holy damage and their body isn't destroyed, they regain half\
    \ their Stamina and fall prone."
"abilities":
- "name": "Razor Claws"
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
    "t1": "2 damage; M1 bleeding (save ends)"
    "t2": "4 damage; M2 bleeding (save ends)"
    "t3": "5 damage; M3 bleeding (save ends) "
- "name": "Leap"
  "type": "Maneuver"
  "keywords":
  - "--"
  "distance": "Self"
  "target": "Self"
  "effects":
  - "name": "Effect"
    "effect": "The ghoul leaps 3 squares. If they land on a size 1 enemy, that enemy\
      \ is knocked prone and the ghoul makes a free strike against them. "

```
