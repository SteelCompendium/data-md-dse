```ds-statblock
"name": "Zombie"
"ancestry":
- "Corporeal"
- "Undead"
"roles":
- "Brute"
"level": !!int "1"
"ev": !!int "10"
"stamina": !!int "20"
"immunities":
- "Corruption 3"
- "Poison 3"
"weaknesses": []
"speed": "6"
"size": "1M"
"stability": !!int "1"
"free_strike": !!int "4"
"might": !!int "2"
"intuition": !!int "-2"
"agility": !!int "1"
"reason": !!int "-5"
"presence": !!int "1"
"traits":
- "name": "Arise"
  "effect": "The first time the zombie is reduced to Stamina 0 by damage that isn't\
    \ fire damage or holy damage and their body isn't destroyed, they regain half\
    \ their Stamina and fall prone."
- "name": "Endless Knight"
  "effect": "The zombie can take advantage of their Arise trait twice."
"abilities":
- "name": "Clobber and Clutch"
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
    "t1": "2 damage; M1 grabbed"
    "t2": "5 damage; M2 grabbed"
    "t3": "6 damage; grabbed"
  - "name": "Effect"
    "effect": "A target who starts their turn grabbed by the zombie takes 2 corruption\
      \ damage. If a creature takes 5 or more corruption damage this way, they become\
      \ insatiably hungry for flesh. The target must complete the Find a Cure project\
      \ to end this effect. "
- "name": "Breakfall"
  "type": "Maneuver"
  "cost": "3 Malice"
  "keywords":
  - "Area"
  - "Resistance"
  "distance": "2 burst"
  "target": "Each enemy in the burst"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 corruption damage"
    "t2": "3 corruption damage; M1 weakened (save ends)"
    "t3": "4 corruption damage; M2 dazed (save ends) "

```
