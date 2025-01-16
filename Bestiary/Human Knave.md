```ds-statblock
"name": "Human Knave"
"ancestry":
- "Human"
- "Humanoid"
"roles":
- "Defender"
"level": !!int "2"
"ev": !!int "18"
"stamina": !!int "50"
"immunities":
- "Magic 2"
- "Psionic 2"
"weaknesses": []
"speed": "5"
"size": "1M"
"stability": !!int "0"
"free_strike": !!int "4"
"might": !!int "2"
"intuition": !!int "0"
"agility": !!int "0"
"reason": !!int "1"
"presence": !!int "0"
"traits":
- "name": "I'm Your Enemy"
  "effect": "The knave can make a free strike against an adjacent creature they have\
    \ taunted whenever the creature deals damage to a creature other than the knave."
- "name": "Overwhelm"
  "effect": "An enemy who starts their turn adjacent to the knave can't shift."
- "name": "Supernatural Insight"
  "effect": "The knave can target supernatural creatures and objects within 5 squares,\
    \ even if they don't have line of effect."
"abilities":
- "name": "Morningstar & Javelin"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Ranged"
  - "Weapon"
  "distance": "Melee 1 or Ranged 5"
  "target": "One creature or object"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "4 damage; M1 the target has a bane on their next attack"
    "t2": "7 damage; M2 the target has a bane on their next attack"
    "t3": "10 damage; M3 the target has a double bane on their next attack"
  - "name": "Effect"
    "effect": "Taunted (EoT). "

```
