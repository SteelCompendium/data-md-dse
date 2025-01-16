```ds-statblock
"name": "Elemental Mote"
"ancestry":
- "Elemental"
- "High Elf"
"roles":
- "Hexer"
- "Minion"
"level": !!int "1"
"ev": !!int "5"
"stamina": !!int "8"
"immunities": []
"weaknesses": []
"speed": "5 (fly)"
"size": "1T"
"stability": !!int "0"
"free_strike": !!int "2"
"might": !!int "0"
"intuition": !!int "0"
"agility": !!int "0"
"reason": !!int "0"
"presence": !!int "2"
"traits":
- "name": "Cradle Heart"
  "effect": "On their turn, the mote can choose to die to revive a dead [[Cradle Crow|cradle crow]],\
    \ [[Cradle Horse|cradle horse]], or [[Cradle Credenza|cradle credenza]] within 1, returning with 8 Stamina."
"abilities":
- "name": "Dweomer Plume"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Magic"
  - "Melee"
  "distance": "Melee 2"
  "target": "1 creature or object per minion"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage"
    "t2": "4 damage; the target gains Magic weakness 1 (EoT)"
    "t3": "5 damage; the target gains Magic weakness 3 (EoT) "

```
