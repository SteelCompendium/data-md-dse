```ds-statblock
"name": "High Elf Orbweaver"
"ancestry":
- "Fey"
- "High Elf"
- "Humanoid"
"roles":
- "Hexer"
"level": !!int "3"
"ev": !!int "16"
"stamina": !!int "35"
"immunities": []
"weaknesses": []
"speed": "5"
"size": "1M"
"stability": !!int "0"
"free_strike": !!int "5"
"might": !!int "0"
"intuition": !!int "2"
"agility": !!int "0"
"reason": !!int "2"
"presence": !!int "2"
"traits":
- "name": "Otherworldly Grace"
  "effect": "At the start of their turn, the orbweaver can turn the duration of one\
    \ save ends effect they suffer from into EoT."
"abilities":
- "name": "Awash"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Area"
  - "Magic"
  "distance": "3 cube within 1"
  "target": "All creatures in the cube"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "3 damage; M1 slowed (EoT)"
    "t2": "4 damage; M2 slowed (EoT)"
    "t3": "5 cold damage; M3 prone "
- "name": "Aetherweb"
  "type": "Action"
  "keywords":
  - "Magic"
  - "Ranged"
  "distance": "Ranged 8"
  "target": "2 enemies or objects"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "3 damage; R1 slowed (save ends)"
    "t2": "5 damage; R2 slowed (save ends)"
    "t3": "6 damage; R3 restrained (save ends)"
  - "name": "Effect"
    "effect": "Each enemy within 3 of a target suffers the same additional effects\
      \ as the target unless they shift into an unoccupied square adjacent to them. "

```
