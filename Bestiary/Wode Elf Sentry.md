```ds-statblock
"name": "Wode Elf Sentry"
"ancestry":
- "Fey"
- "Humanoid"
- "Wode Elf"
"roles":
- "Support"
"level": !!int "1"
"ev": !!int "13"
"stamina": !!int "30"
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
  "effect": "The sentry immediately hides at the end of their turn while in cover\
    \ or concealment, even if they are observed."
"abilities":
- "name": "Tracer Longbow"
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
    "t1": "3 damage; A2 marked (save ends)"
    "t2": "5 damage; A3 marked (save ends)"
    "t3": "7 damage; marked (save ends)"
  - "name": "Effect"
    "effect": "Allies have **+1** on attacks and abilities against marked creatures\
      \ and objects."
  - "name": "3 Malice"
    "effect": "The sentry targets two additional creatures or objects. "
- "name": "Death Blossom"
  "type": "Maneuver"
  "cost": "2 Malice"
  "keywords":
  - "Area"
  - "Weapon"
  "distance": "5 burst"
  "target": "All marked enemies"
  "effects":
  - "name": "Effect"
    "effect": "3 damage. "

```
