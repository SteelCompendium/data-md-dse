```ds-statblock
"name": "Cradle Horse"
"ancestry":
- "Construct"
- "High Elf"
"roles":
- "Mount"
"level": !!int "1"
"ev": !!int "13"
"stamina": !!int "30"
"immunities": []
"weaknesses": []
"speed": "10"
"size": "2"
"stability": !!int "2"
"free_strike": !!int "3"
"might": !!int "2"
"intuition": !!int "0"
"agility": !!int "2"
"reason": !!int "0"
"presence": !!int "1"
"traits":
- "name": "Shared Otherworldly Grace"
  "effect": "If the cradle horse's rider has the Otherworldly Grace trait, it also\
    \ gains the Otherworldly Grace trait."
"abilities":
- "name": "Radiant Charge"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Charge"
  - "Melee"
  - "Weapon"
  "distance": "Melee 1"
  "target": "1 creature or object"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "3 damage; M1 prone"
    "t2": "5 fire damage; M2 prone"
    "t3": "7 lightning damage; M3 prone "
- "name": "Stomp"
  "type": "Action"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "1 burst"
  "target": "All enemies in the burst"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage"
    "t2": "4 damage"
    "t3": "5 damage"
  - "name": "Effect"
    "effect": "This attack has edge against prone targets. "
- "name": "Buck"
  "type": "Maneuver"
  "cost": "2 Malice"
  "keywords":
  - "--"
  "distance": "Self"
  "target": "The horse's rider"
  "effects":
  - "name": "Effect"
    "effect": "Vertical slide 3; The rider can use a ranged ability at any point during\
      \ the movement and then fall without taking damage. "

```
