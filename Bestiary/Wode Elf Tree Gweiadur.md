```ds-statblock
"name": "Wode Elf Tree Gweiadur"
"ancestry":
- "Fey"
- "Humanoid"
- "Wode Elf"
"roles":
- "Artillery"
"level": !!int "3"
"ev": !!int "17"
"stamina": !!int "35"
"immunities": []
"weaknesses": []
"speed": "7"
"size": "1M"
"stability": !!int "0"
"free_strike": !!int "5"
"might": !!int "0"
"intuition": !!int "1"
"agility": !!int "2"
"reason": !!int "0"
"presence": !!int "0"
"traits":
- "name": "Masking Glamor"
  "effect": "The tree gweiadur immediately hides at the end of their turn while in\
    \ cover or concealment, even if they are observed."
"abilities":
- "name": "Snare Bow"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Ranged"
  - "Weapon"
  "distance": "Ranged 15"
  "target": "1 creature or object"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "5 damage; A1 restrained (save ends)"
    "t2": "9 damage; A2 restrained (save ends)"
    "t3": "12 damage; A3 restrained (save ends)"
  - "name": "Effect"
    "effect": "The tree gweiadur can shift 3 after making the attack."
  - "name": "3 Malice"
    "effect": "If this attack restrains the target, an enemy within 1 of the target\
      \ is also restrained (save ends). "
- "name": "You Activated My Trap!"
  "type": "Maneuver"
  "cost": "3 Malice"
  "keywords":
  - "Area"
  - "Magic"
  - "Ranged"
  "distance": "3 cube within 10"
  "target": "All enemies in the cube"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage; R1 marked (save ends)"
    "t2": "4 damage; R2 slowed and marked (save ends)"
    "t3": "6 damage; R3 slowed and marked (save ends)"
  - "name": "Effect"
    "effect": "Allies have **+1** on attacks and abilities against marked creatures\
      \ and objects. "

```
