```ds-statblock
"name": "Human Archer"
"ancestry":
- "Human"
- "Humanoid"
"roles":
- "Artillery"
- "Minion"
"level": !!int "1"
"ev": !!int "6"
"stamina": !!int "8"
"immunities":
- "Magic 2"
- "Psionic 2"
"weaknesses": []
"speed": "5"
"size": "1M"
"stability": !!int "0"
"free_strike": !!int "2"
"might": !!int "0"
"intuition": !!int "0"
"agility": !!int "2"
"reason": !!int "0"
"presence": !!int "0"
"traits":
- "name": "Supernatural Insight"
  "effect": "The archer can target supernatural creatures and objects within 5 squares,\
    \ even if they don't have line of effect."
"abilities":
- "name": "Crossbow"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Ranged"
  - "Weapon"
  "distance": "Ranged 15"
  "target": "One creature or object per minion"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage"
    "t2": "5 damage"
    "t3": "6 damage "

```
