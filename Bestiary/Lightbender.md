```ds-statblock
"name": "Lightbender"
"ancestry":
- "Lightbender"
- "Monster"
"roles":
- "Ambusher"
"level": !!int "3"
"ev": !!int "38"
"stamina": !!int "80"
"immunities": []
"weaknesses": []
"speed": "10"
"size": "2"
"stability": !!int "1"
"free_strike": !!int "5"
"might": !!int "2"
"intuition": !!int "0"
"agility": !!int "1"
"reason": !!int "-3"
"presence": !!int "-1"
"traits":
- "name": "Avoidance"
  "effect": "The lightbender always treats a save-ends effect as an EoT effect."
"abilities":
- "name": "Sucker Swipe"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "Melee 2"
  "target": "1 creature or object"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "8 damage"
    "t2": "12 damage"
    "t3": "16 damage"
  - "name": "Effect"
    "effect": "The lightbender has advantage on the attack if they would make it with\
      \ an edge. "
- "name": "Piercing Tails"
  "type": "Action"
  "keywords":
  - "Attack"
  - "Melee"
  - "Weapon"
  "distance": "Melee 2"
  "target": "2 creatures or objects"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "6 damage; 1 bleeding (save ends)"
    "t2": "10 damage; 2 bleeding (save ends)"
    "t3": "13 damage; 3 bleeding (save ends)"
  - "name": "Effect"
    "effect": "A creature who is bleeding from this ability has a bane on tests to\
      \ search for the lightbender until the condition ends. "
- "name": "Hypnotic Mane"
  "type": "Maneuver"
  "cost": "5 Malice"
  "keywords":
  - "Area"
  - "Magic"
  - "Resistance"
  "distance": "3 burst"
  "target": "All enemies in the burst"
  "effects":
  - "roll": "INU RR"
    "t1": "Dazed (save ends)"
    "t2": "Dazed (EoT)"
    "t3": "No effect"
  - "name": "Effect"
    "effect": "Targets dazed by this ability have a speed of 0 while dazed. If a dazed\
      \ target takes damage or if someone else spends an action to shake the creature\
      \ out of their stupor, the condition is removed. "
- "name": "Stalker's Afterimage"
  "type": "Triggered Action"
  "keywords":
  - "Magic"
  "trigger": "The lightbender is damaged by an attack"
  "distance": "Self"
  "target": "Self"
  "effects":
  - "name": "Effect"
    "effect": "The lightbender halves the damage, doesn't suffer any associated effect,\
      \ and teleports 5 squares. The lightbender immediately hides if they teleport\
      \ into cover or concealment. "

```
