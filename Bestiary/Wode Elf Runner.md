```ds-statblock
"name": "Wode Elf Runner"
"ancestry":
- "Fey"
- "Humanoid"
- "Wode Elf"
"roles":
- "Harrier"
- "Minion"
"level": !!int "1"
"ev": !!int "6"
"stamina": !!int "10"
"immunities": []
"weaknesses": []
"speed": "7"
"size": "1M"
"stability": !!int "0"
"free_strike": !!int "2"
"might": !!int "0"
"intuition": !!int "0"
"agility": !!int "2"
"reason": !!int "0"
"presence": !!int "1"
"traits":
- "name": "Masking Glamor"
  "effect": "The runner immediately hides at the end of their turn while in cover\
    \ or concealment, even if they are observed."
"abilities":
- "name": "Spear"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Charge"
  - "Melee"
  - "Ranged"
  - "Weapon"
  "distance": "Melee 1 or Ranged 5"
  "target": "1 creature or object per minion"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage"
    "t2": "4 damage"
    "t3": "5 damage"
  - "name": "Effect"
    "effect": "The runner can shift 2 before making the attack. "

```
