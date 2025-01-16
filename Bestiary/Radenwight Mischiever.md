```ds-statblock
"name": "Radenwight Mischiever"
"ancestry":
- "Humanoid"
- "Radenwight"
"roles":
- "Ambusher"
- "Minion"
"level": !!int "1"
"ev": !!int "7"
"stamina": !!int "10"
"immunities": []
"weaknesses": []
"speed": "7 (climb)"
"size": "1S"
"stability": !!int "0"
"free_strike": !!int "2"
"might": !!int "-1"
"intuition": !!int "0"
"agility": !!int "2"
"reason": !!int "0"
"presence": !!int "0"
"traits": []
"abilities":
- "name": "Dagger Dance"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "Melee 1 or Ranged 5"
  "target": "One creature per minion"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage"
    "t2": "5 damage"
    "t3": "6 damage"
  - "name": "Effect"
    "effect": "If the mischief is hidden when they use this ability, they can target\
      \ two creatures. "
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
    "effect": "The mischief makes a free strike against the target."

```
