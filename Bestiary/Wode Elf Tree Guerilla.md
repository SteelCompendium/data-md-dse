```ds-statblock
"name": "Wode Elf Tree Guerilla"
"ancestry":
- "Fey"
- "Humanoid"
- "Wode Elf"
"roles":
- "Ambusher"
"level": !!int "3"
"ev": !!int "19"
"stamina": !!int "45"
"immunities": []
"weaknesses": []
"speed": "7 (teleport)"
"size": "1M"
"stability": !!int "0"
"free_strike": !!int "5"
"might": !!int "0"
"intuition": !!int "0"
"agility": !!int "2"
"reason": !!int "0"
"presence": !!int "1"
"traits":
- "name": "Hunter's Glamor"
  "effect": "The tree guerilla immediately hides at the end of their turn, even if\
    \ they are observed."
"abilities":
- "name": "Splinter Dagger"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Ranged"
  - "Weapon"
  "distance": "Melee 1 or Ranged 5"
  "target": "1 creature or object"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "5 damage; M1 bleeding (save ends)"
    "t2": "9 damage; M2 bleeding (save ends)"
    "t3": "12 damage; M3 bleeding (save ends)"
  - "name": "Effect"
    "effect": "The tree guerilla can teleport 3 after making the attack."
  - "name": "5 Malice"
    "effect": "The tree guerilla targets an additional creature or object. The tree\
      \ guerilla has **+1** if both targets are adjacent to each other. "
- "name": "Do Not Hesitate in the Wode"
  "type": "Free Triggered Action"
  "cost": "3 Malice"
  "keywords":
  - "--"
  "distance": "Self and Squad"
  "target": "Self and Squad"
  "trigger": "An ally ends their turn while the tree guerilla hasn't acted this round."
  "effects":
  - "name": "Effect"
    "effect": "The targets take their turn immediately. Each target has **+1** until\
      \ the end of their turn. "

```
