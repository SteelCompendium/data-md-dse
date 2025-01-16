```ds-statblock
"name": "Bugbear Commander"
"ancestry":
- "Bugbear"
- "Goblin"
- "Humanoid"
"roles":
- "SUPPORT"
"level": !!int "2"
"ev": !!int "32"
"stamina": !!int "70"
"immunities": []
"weaknesses": []
"speed": "5"
"size": "1M"
"stability": !!int "0"
"free_strike": !!int "5"
"might": !!int "2"
"intuition": !!int "0"
"agility": !!int "1"
"reason": !!int "2"
"presence": !!int "0"
"traits":
- "name": "The Commander's Watching"
  "effect": "While an ally has line of effect to the commander, the ally can end one\
    \ condition afflicting them at the start of their turn."
"abilities":
- "name": "Inspiring Swordplay"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "Melee 1"
  "target": "2 creatures or objects"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "5 damage"
    "t2": "8 damage"
    "t3": "11 damage; one target is grabbed"
  - "name": "Effect"
    "effect": "1 ally within 5 of the commander has an edge on their next attack until\
      \ the start of the commander's next turn. "
- "name": "You Next!"
  "type": "Action"
  "keywords":
  - "--"
  "distance": "Ranged 8"
  "target": "1 ally"
  "effects":
  - "name": "Effect"
    "effect": "The target moves up to their speed and uses a signature action. "
- "name": "Fall Back!"
  "type": "Action"
  "cost": "5 Malice"
  "keywords":
  - "--"
  "distance": "Self and 5 burst"
  "target": "Self and all allies"
  "effects":
  - "name": "Effect"
    "effect": "Each target shifts up to their speed. One target can then use the Throw\
      \ maneuver if they have it. "
- "name": "Throw"
  "type": "Maneuver"
  "keywords":
  - "Attack"
  - "Melee"
  "distance": "Melee 1"
  "target": "1 creature or object grabbed by the commander"
  "effects":
  - "name": "Effect"
    "effect": "Vertical push 4; ally targets don't take damage from being force moved. "
- "name": "Catcher"
  "type": "Free Triggered Action"
  "keywords":
  - "--"
  "distance": "Melee 1"
  "target": "1 size 1 creature or object"
  "trigger": "The target is force moved into a square adjacent to the commander."
  "effects":
  - "name": "Effect"
    "effect": "The target is grabbed by the commander. "

```
