```ds-statblock
"name": "Human Brawler"
"ancestry":
- "Human"
- "Humanoid"
"roles":
- "Brute"
"level": !!int "1"
"ev": !!int "16"
"stamina": !!int "40"
"immunities":
- "Magic 2"
- "Psionic 2"
"weaknesses": []
"speed": "5"
"size": "1M"
"stability": !!int "0"
"free_strike": !!int "4"
"might": !!int "2"
"intuition": !!int "0"
"agility": !!int "1"
"reason": !!int "0"
"presence": !!int "0"
"traits":
- "name": "Shoot the Hostage"
  "effect": "The brawler takes half damage from attacks if they have a creature or\
    \ object grabbed. The grabbed creature or object takes the other half of the damage."
- "name": "Supernatural Insight"
  "effect": "The brawler can target supernatural creatures and objects within 5 squares,\
    \ even if they don't have line of effect."
"abilities":
- "name": "Haymaker"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "Melee 1"
  "target": "One creature or object"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "4 damage; M1 grabbed"
    "t2": "7 damage; M2 grabbed"
    "t3": "10 damage; M3 grabbed"
  - "name": "Effect"
    "effect": "The target has a bane on attempts to escape the grab. The brawler has\
      \ edge on this attack if the target is already grabbed. "
- "name": "Throw"
  "type": "Maneuver"
  "cost": "1 Malice"
  "keywords":
  - "--"
  "distance": "Melee 1"
  "target": "One creature grabbed by the brawler"
  "effects":
  - "name": "Effect"
    "effect": "Push 5. "

```
