```ds-statblock
"name": "Dwarf Shieldwall"
"ancestry":
- "Dwarf"
- "Humanoid"
"roles":
- "Defender"
"level": !!int "3"
"ev": !!int "16"
"stamina": !!int "70"
"immunities":
- "weapon 3"
"weaknesses": []
"speed": "5"
"size": "1M"
"stability": !!int "4"
"free_strike": !!int "5"
"might": !!int "2"
"intuition": !!int "0"
"agility": !!int "0"
"reason": !!int "0"
"presence": !!int "1"
"traits":
- "name": "Call to the Wall"
  "effect": "The shieldwall inflicts taunted (EoT) on a creature whenever they deal\
    \ damage to the shieldwall or take damage from the shieldwall."
"abilities":
- "name": "Wide Axe"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "Melee 1"
  "target": "1 creature or object"
  "effects":
  - "roll": "2d10 + 1"
    "t1": "5 damage; slide 1"
    "t2": "8 damage; slide 1"
    "t3": "11 damage; slide 1"
  - "name": "Effect"
    "effect": "The shieldwall can shift 1 to remain adjacent to the target. A target\
      \ restrained by a dwarf can be slid by this attack."
  - "name": "3 Malice"
    "effect": "The shieldwall targets an additional creature or object. "
- "name": "Intercepting Shield"
  "type": "Triggered Action"
  "cost": "1 Malice"
  "keywords":
  - "--"
  "distance": "Self"
  "target": "Self"
  "trigger": "A creature attacks an adjacent ally."
  "effects":
  - "name": "Effect"
    "effect": "The shieldwall becomes the attack's target and has +3 defense against\
      \ it. "

```
