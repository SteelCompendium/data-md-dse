```ds-statblock
"name": "Rotting [[Zombie]]"
"ancestry":
- "Corporeal"
- "Undead"
"roles":
- "Brute"
- "Minion"
"level": !!int "1"
"ev": !!int "4"
"stamina": !!int "8"
"immunities":
- "Corruption 2"
- "Poison 2"
"weaknesses": []
"speed": "6"
"size": "1M"
"stability": !!int "0"
"free_strike": !!int "2"
"might": !!int "2"
"intuition": !!int "-2"
"agility": !!int "-2"
"reason": !!int "-5"
"presence": !!int "-3"
"traits":
- "name": "Arise Together"
  "effect": "If the rotting [[Zombie|zombie]]'s captain has the Arise trait, the [[Zombie|zombie]] also\
    \ gains the Arise trait."
"abilities":
- "name": "Rotting Fist"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "Melee 1"
  "target": "One creature or object per minion"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage"
    "t2": "3 damage; M1 slowed (save ends)"
    "t3": "4 damage; M2 prone if size 1, slowed (save ends) otherwise "

```
