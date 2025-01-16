```ds-statblock
"name": "Human Scoundrel"
"ancestry":
- "Human"
- "Humanoid"
"roles":
- "Ambusher"
"level": !!int "1"
"ev": !!int "14"
"stamina": !!int "30"
"immunities":
- "Magic 2"
- "Psionic 2"
"weaknesses": []
"speed": "5"
"size": "1M"
"stability": !!int "0"
"free_strike": !!int "4"
"might": !!int "0"
"intuition": !!int "0"
"agility": !!int "2"
"reason": !!int "0"
"presence": !!int "1"
"traits":
- "name": "Supernatural Insight"
  "effect": "The scoundrel can target supernatural creatures and objects within 5\
    \ squares, even if they don't have line of effect."
"abilities":
- "name": "Rapier & Dagger"
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
    "t1": "4 damage"
    "t2": "7 damage"
    "t3": "10 damage"
  - "name": "Effect"
    "effect": "This ability has double edge if the scoundrel has an edge on the power\
      \ roll. "
- "name": "Dagger Storm"
  "type": "Action"
  "cost": "5 Malice"
  "effects":
  - "name": "Effect"
    "effect": "The scoundrel makes a Rapier & Dagger attack against three creatures\
      \ or objects. They can shift 2 squares before or after each attack. "

```
