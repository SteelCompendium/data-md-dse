```ds-statblock
"name": "Dwarf Gunner"
"ancestry":
- "Dwarf"
- "Humanoid"
"roles":
- "Artillery"
"level": !!int "1"
"ev": !!int "12"
"stamina": !!int "26"
"immunities": []
"weaknesses": []
"speed": "5"
"size": "1M"
"stability": !!int "1"
"free_strike": !!int "3"
"might": !!int "0"
"intuition": !!int "1"
"agility": !!int "2"
"reason": !!int "0"
"presence": !!int "0"
"traits":
- "name": "Split Shot"
  "effect": "Whenever the gunner deals damage to a creature or object, a creature\
    \ or object within 1 of the recipient takes 3 damage."
"abilities":
- "name": "Portable Ballista"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Ranged"
  - "Weapon"
  "distance": "Ranged 10"
  "target": "1 creature or object"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "4 damage; push 1"
    "t2": "7 damage; push 3"
    "t3": "10 damage; push 5"
  - "name": "Effect"
    "effect": "If the target is adjacent to a wall or object after the power roll\
      \ is resolved, they are restrained (EoT). A target restrained by a dwarf can\
      \ be pushed by this attack."
  - "name": "5 Malice"
    "effect": "If the target is pushed into another creature, both the target and\
      \ the creature are restrained (EoT). "
- "name": "Ensnaring Chains"
  "type": "Maneuver"
  "cost": "5 Malice"
  "keywords":
  - "Ranged"
  - "Weapon"
  "distance": "Ranged 10"
  "target": "1 restrained, slowed, or prone target"
  "effects":
  - "name": "Effect"
    "effect": "The gunner makes a free strike against the target. The target loses\
      \ any restrained, slowed, or prone conditions and gains restrained (save ends). "

```
