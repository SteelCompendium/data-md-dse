```ds-statblock
"name": "War Dog Tetherite"
"ancestry":
- "Humanoid"
- "War Dog"
"roles":
- "Brute"
- "Minion"
"level": !!int "1"
"ev": !!int "6"
"stamina": !!int "8"
"immunities": []
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
- "name": "Tethered"
  "effect": "A captain attached to a tetherite squad has their Stability increased\
    \ by the number of tetherites within 2 squares of them."
- "name": "Loyalty Collar"
  "effect": "When the tetherite dies, they explode, dealing 1d6 damage to each adjacent\
    \ enemy."
"abilities":
- "name": "Banded Dagger"
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
    "t2": "4 damage"
    "t3": "5 damage "

```
