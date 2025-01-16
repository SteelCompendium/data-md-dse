```ds-statblock
"name": "Human Apprentice Mage"
"ancestry":
- "Human"
- "Humanoid"
"roles":
- "Controller"
- "Minion"
"level": !!int "2"
"ev": !!int "6"
"stamina": !!int "10"
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
"agility": !!int "1"
"reason": !!int "0"
"presence": !!int "2"
"traits":
- "name": "Studied Supernatural Insight"
  "effect": "The apprentice can target supernatural creatures and objects within 10\
    \ squares, even if they don't have line of effect."
"abilities":
- "name": "Lightning Strike"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Magic"
  - "Ranged"
  "distance": "Ranged 10"
  "target": "One creature or object per minion"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 lightning damage"
    "t2": "4 lightning damage"
    "t3": "5 lightning damage"
  - "name": "Effect"
    "effect": "If the apprentice mage doesn't use a maneuver or a move action this\
      \ turn, the target is slowed (EoT). "

```
