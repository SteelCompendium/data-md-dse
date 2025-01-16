```ds-statblock
"name": "Goblin Assassin"
"ancestry":
- "Goblin"
- "Humanoid"
"roles":
- "Ambusher"
"level": !!int "1"
"ev": !!int "11"
"stamina": !!int "20"
"immunities": []
"weaknesses": []
"speed": "6 (climb)"
"size": "1S"
"stability": !!int "0"
"free_strike": !!int "3"
"might": !!int "-2"
"intuition": !!int "0"
"agility": !!int "2"
"reason": !!int "0"
"presence": !!int "-2"
"traits":
- "name": "Crafty"
  "effect": "The assassin doesn't provoke opportunity attacks by moving."
- "name": "Hide While Observed"
  "effect": "The assassin can take the Hide maneuver even while observed, though they\
    \ still must have cover or concealment."
"abilities":
- "name": "Sword"
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
    "t1": "3 damage"
    "t2": "5 damage"
    "t3": "7 damage"
  - "name": "Effect"
    "effect": "This ability has edge if the assassin has an edge on the power roll. "
- "name": "Shadow Chains"
  "type": "Action"
  "cost": "3 Malice"
  "keywords":
  - "Magic"
  - "Ranged"
  "distance": "Ranged 10"
  "target": "Three creatures"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "3 corruption damage; A1 restrained (save ends)"
    "t2": "5 corruption damage; A2 restrained (save ends)"
    "t3": "7 corruption damage; A3 restrained (save ends) "

```
