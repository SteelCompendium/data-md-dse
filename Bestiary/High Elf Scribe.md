```ds-statblock
"name": "High Elf Scribe"
"ancestry":
- "Fey"
- "High Elf"
- "Humanoid"
"roles":
- "Controller"
- "Minion"
"level": !!int "1"
"ev": !!int "5"
"stamina": !!int "8"
"immunities": []
"weaknesses": []
"speed": "5"
"size": "1M"
"stability": !!int "0"
"free_strike": !!int "2"
"might": !!int "0"
"intuition": !!int "1"
"agility": !!int "0"
"reason": !!int "1"
"presence": !!int "1"
"traits":
- "name": "Otherworldly Grace"
  "effect": "At the start of their turn, the scribe can turn the duration of one save\
    \ ends effect they suffer from into EoT."
"abilities":
- "name": "Inkshot"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Magic"
  - "Ranged"
  "distance": "Ranged 5"
  "target": "1 creature or object per minion"
  "effects":
  - "roll": "2d10 + 1"
    "t1": "2 corruption damage"
    "t2": "4 corruption damage"
    "t3": "5 corruption damage"
  - "name": "Effect"
    "effect": "The next attack made against the target before the start of the scribe's\
      \ next turn has edge. "

```
