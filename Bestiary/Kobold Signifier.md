```ds-statblock
"name": "Kobold Signifier"
"ancestry":
- "Humanoid"
- "Kobold"
"roles":
- "Support"
"level": !!int "1"
"ev": !!int "8"
"stamina": !!int "15"
"immunities": []
"weaknesses": []
"speed": "5"
"size": "1S"
"stability": !!int "0"
"free_strike": !!int "1"
"might": !!int "0"
"intuition": !!int "0"
"agility": !!int "1"
"reason": !!int "0"
"presence": !!int "2"
"traits":
- "name": "Upholding High Standards"
  "effect": "Allies within 5 of the signifier have an edge and resistance. If the\
    \ signifier is killed, a minion from their squad can retrieve the signum and replace\
    \ their stat block with the signifier stat block."
- "name": "Shield? Shield!"
  "effect": "The signifier has increased Stability by 1 and can act as cover for allies\
    \ when adjacent to an ally who also has this trait."
"abilities":
- "name": "Signum"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "Melee 1"
  "target": "1 creature or object"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "2 damage"
    "t2": "4 damage"
    "t3": "5 damage"
  - "name": "Effect"
    "effect": "An ally within 10 can shift their speed, as long as they end their\
      \ movement adjacent to an ally."
  - "name": "2+ Malice"
    "effect": "1 additional ally can shift for every 2 malice spent. "
- "name": "Glory to the Legion"
  "type": "Maneuver"
  "cost": "5 Malice"
  "keywords":
  - "Area"
  "distance": "5 burst"
  "target": "All allies in the burst"
  "effects":
  - "name": "Effect"
    "effect": "Each target regains 5 Stamina. "

```
