```ds-statblock
"name": "Human Death Acolyte"
"ancestry":
- "Human"
- "Humanoid"
"roles":
- "Hexer"
- "Minion"
"level": !!int "1"
"ev": !!int "5"
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
"agility": !!int "1"
"reason": !!int "0"
"presence": !!int "2"
"traits":
- "name": "Supernatural Insight"
  "effect": "The death acolyte can target supernatural creatures and objects within\
    \ 5 squares, even if they don't have line of effect."
"abilities":
- "name": "Necrotic Bolt"
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
    "t1": "2 corruption damage"
    "t2": "4 corruption damage"
    "t3": "5 corruption damage"
  - "name": "Effect"
    "effect": "A creature within 5 squares of the death acolyte regains 1 Stamina. "

```
