```ds-statblock
"name": "War Dog Pestilite"
"ancestry":
- "Humanoid"
- "War Dog"
"roles":
- "Controller"
"level": !!int "3"
"ev": !!int "13"
"stamina": !!int "25"
"immunities":
- "Poison 3"
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
- "name": "Loyalty Collar"
  "effect": "When the pestilite dies, they explode, dealing 1d6 damage to each adjacent\
    \ enemy."
"abilities":
- "name": "Plaguecaster"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Area"
  - "Magic"
  - "Ranged"
  - "Resistance"
  "distance": "3 cube within 10"
  "target": "Each creature in the cube"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 poison damage; I1 frightened (save ends)"
    "t2": "5 poison damage; I2 frightened (save ends)"
    "t3": "8 poison damage; I3 frightened (save ends)"
  - "name": "Effect"
    "effect": "The area is covered in a cloud of pestilence that lasts until the start\
      \ of the pestilite's next turn. Any creature who enters the area for the first\
      \ time in a round or starts their turn there takes 2 poison damage. "
- "name": "Posthumous Promotion"
  "type": "Maneuver"
  "keywords":
  - "Magic"
  - "Ranged"
  "distance": "Ranged 10"
  "target": "One war dog with a loyalty collar"
  "effects":
  - "name": "Effect"
    "effect": "The target's loyalty collar detonates, killing them instantly. "

```
