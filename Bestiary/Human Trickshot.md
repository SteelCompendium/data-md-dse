```ds-statblock
"name": "Human Trickshot"
"ancestry":
- "Human"
- "Humanoid"
"roles":
- "Artillery"
"level": !!int "1"
"ev": !!int "12"
"stamina": !!int "20"
"immunities":
- "Magic 2"
- "Psionic 2"
"weaknesses": []
"speed": "5"
"size": "1M"
"stability": !!int "0"
"free_strike": !!int "4"
"might": !!int "0"
"intuition": !!int "1"
"agility": !!int "2"
"reason": !!int "0"
"presence": !!int "0"
"traits":
- "name": "Supernatural Insight"
  "effect": "The trickshot can target supernatural creatures and objects within 5\
    \ squares, even if they don't have line of effect."
"abilities":
- "name": "Trick Crossbow"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Ranged"
  - "Weapon"
  "distance": "Melee 1 or Ranged 15"
  "target": "One creature or object"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "4 damage"
    "t2": "7 damage"
    "t3": "10 damage"
  - "name": "Effect"
    "effect": "The trickshot ignores cover and concealment."
  - "name": "3 Malice"
    "effect": "The trickshot attacks an additional target. "

```
