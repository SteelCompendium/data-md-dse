```ds-statblock
"name": "Human Guard"
"ancestry":
- "Human"
- "Humanoid"
"roles":
- "Brute"
- "Minion"
"level": !!int "1"
"ev": !!int "6"
"stamina": !!int "12"
"immunities":
- "Magic 2"
- "Psionic 2"
"weaknesses": []
"speed": "5"
"size": "1M"
"stability": !!int "0"
"free_strike": !!int "2"
"might": !!int "2"
"intuition": !!int "0"
"agility": !!int "0"
"reason": !!int "0"
"presence": !!int "0"
"traits":
- "name": "Supernatural Insight"
  "effect": "The guard can target supernatural creatures and objects within 5 squares,\
    \ even if they don't have line of effect."
"abilities":
- "name": "Halberd"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "Melee 2"
  "target": "One creature or object per minion"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage"
    "t2": "5 damage"
    "t3": "6 damage"
  - "name": "Effect"
    "effect": "If the guard is flanked, they can make a free strike against an additional\
      \ target adjacent to them. "

```
