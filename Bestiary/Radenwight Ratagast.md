```ds-statblock
"name": "Radenwight Ratagast"
"ancestry":
- "Humanoid"
- "Radenwight"
"roles":
- "Defender"
- "Minion"
"level": !!int "1"
"ev": !!int "7"
"stamina": !!int "12"
"immunities": []
"weaknesses": []
"speed": "6 (climb)"
"size": "1S"
"stability": !!int "0"
"free_strike": !!int "2"
"might": !!int "-1"
"intuition": !!int "0"
"agility": !!int "1"
"reason": !!int "0"
"presence": !!int "2"
"traits": []
"abilities":
- "name": "Stinky Glissando"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Magic"
  - "Melee"
  "distance": "Melee 1"
  "target": "One creature or object per minion"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 poison damage"
    "t2": "4 poison damage; taunted (EoT)"
    "t3": "5 poison damage; taunted (EoT) "
- "name": "Ready Rodent"
  "type": "Triggered Action"
  "keywords":
  - "Melee"
  - "Weapon"
  "distance": "Melee 1"
  "target": "One creature"
  "trigger": "An ally deals damage to the target."
  "effects":
  - "name": "Effect"
    "effect": "The ratagast makes a free strike against the target."

```
