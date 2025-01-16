```ds-statblock
"name": "Dwarf Reel Winch"
"ancestry":
- "Dwarf"
- "Humanoid"
"roles":
- "Support"
"level": !!int "1"
"ev": !!int "13"
"stamina": !!int "36"
"immunities": []
"weaknesses": []
"speed": "5"
"size": "1M"
"stability": !!int "2"
"free_strike": !!int "3"
"might": !!int "0"
"intuition": !!int "1"
"agility": !!int "2"
"reason": !!int "0"
"presence": !!int "0"
"traits":
- "name": "We Have a Quota!"
  "effect": "If the engineer applies the slowed condition to a target who is already\
    \ slowed or grabbed, the target becomes restrained (save ends) and the slowed\
    \ or grabbed condition ends."
"abilities":
- "name": "Snaring Crossbow"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Ranged"
  - "Weapon"
  "distance": "Ranged 10"
  "target": "1 creature or object"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "3 damage; M1 slowed (save ends)"
    "t2": "5 damage; M2 slowed (save ends)"
    "t3": "7 damage; M3 restrained (save ends)"
  - "name": "2 Malice"
    "effect": "Pull 5. A target restrained by a dwarf, including by this ability,\
      \ can be pulled this way. "
- "name": "Reel Them In"
  "type": "Maneuver"
  "cost": "3 Malice"
  "keywords":
  - "Ranged"
  - "Weapon"
  "distance": "Ranged 10"
  "target": "3 creatures"
  "effects":
  - "name": "Effect"
    "effect": "Pull 5. A slowed or restrained target is pulled an additional 2. A\
      \ target restrained by a dwarf can be pulled this way. "

```
