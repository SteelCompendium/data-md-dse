```ds-statblock
"name": "High Elf Quiver"
"ancestry":
- "Fey"
- "High Elf"
- "Humanoid"
"roles":
- "Artillery"
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
"might": !!int "0"
"intuition": !!int "0"
"agility": !!int "2"
"reason": !!int "1"
"presence": !!int "0"
"traits":
- "name": "Otherworldly Grace"
  "effect": "At the start of their turn, the quiver can turn the duration of one save\
    \ ends effect they suffer from into EoT."
"abilities":
- "name": "Heavy Arrow"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Ranged"
  - "Weapon"
  "distance": "Ranged 10"
  "target": "1 creature or object per minion"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage"
    "t2": "5 damage; target's speed reduced by 1 (EoT)"
    "t3": "6 damage; target's speed reduced by 2 (EoT) "

```
