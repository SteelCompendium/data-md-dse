```ds-statblock
"name": "[[Dwarf]] Grenadier"
"ancestry":
- "[[Dwarf]]"
- "Humanoid"
"roles":
- "Hexer"
"level": !!int "2"
"ev": !!int "13"
"stamina": !!int "33"
"immunities": []
"weaknesses": []
"speed": "5"
"size": "1M"
"stability": !!int "3"
"free_strike": !!int "4"
"might": !!int "1"
"intuition": !!int "2"
"agility": !!int "0"
"reason": !!int "0"
"presence": !!int "0"
"traits":
- "name": "Indirect Fire"
  "effect": "The grenadier ignores cover and concealment and doesn't need to establish\
    \ line of effect for their abilities."
"abilities":
- "name": "Concussive Grenade"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Area"
  - "Ranged"
  - "Weapon"
  "distance": "3 cube within 5"
  "target": "All enemies"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "3 damage; push 1; M1 [[Slowed|slowed]] (save ends)"
    "t2": "5 damage; push 3; M2 [[Slowed|slowed]] (save ends)"
    "t3": "7 damage; push 5; M3 [[Slowed|slowed]] (save ends)"
  - "name": "Effect"
    "effect": "A target [[Restrained|restrained]] by a [[Dwarf|dwarf]] can be pushed by this ability. "
- "name": "Sleep Grenade"
  "type": "Action"
  "cost": "3 Malice"
  "keywords":
  - "Area"
  - "Ranged"
  "distance": "3 cube within 5"
  "target": "All enemies"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "3 poison damage; I1 [[Dazed|dazed]] (save ends)"
    "t2": "5 poison damage; I2 [[Dazed|dazed]] (save ends)"
    "t3": "7 poison damage; I3 [[Dazed|dazed]] (save ends)"
  - "name": "Effect"
    "effect": "A creature [[Dazed|dazed]] by this ability has -1 to all characteristics while\
      \ resisting potent effects until the condition ends. "

```
