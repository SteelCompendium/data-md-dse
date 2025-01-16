```ds-statblock
"name": "Gnoll Abyssal Summoner"
"ancestry":
- "Fiend"
- "Gnoll"
"roles":
- "Support"
"level": !!int "2"
"ev": !!int "12"
"stamina": !!int "25"
"immunities": []
"weaknesses": []
"speed": "5"
"size": "1M"
"stability": !!int "1"
"free_strike": !!int "3"
"might": !!int "1"
"intuition": !!int "2"
"agility": !!int "0"
"reason": !!int "0"
"presence": !!int "2"
"traits":
- "name": "Death Frenzy"
  "effect": "Whenever an ally within 5 is reduced to 0 Stamina, the abyssal summoner\
    \ moves up to their speed and makes a free strike."
"abilities":
- "name": "Flame Wad"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Attack"
  - "Magic"
  - "Ranged"
  "distance": "Ranged 5"
  "target": "1 creature or object"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "3 fire damage; I1 burning (save ends)"
    "t2": "5 fire damage; I2 burning (save ends)"
    "t3": "7 fire damage; I3 burning (save ends)"
  - "name": "Effect"
    "effect": "A burning target takes 1d6 fire damage at the start of each of their\
      \ turns until the condition ends. "
- "name": "Call [[Abyssal Hyena|Abyssal Hyenas]]"
  "type": "Maneuver"
  "cost": "3 Malice"
  "keywords":
  - "--"
  "distance": "Ranged 5"
  "target": "Special"
  "effects":
  - "name": "Effect"
    "effect": "2 [[Abyssal Hyena|abyssal hyenas]] claw out of the ground into unoccupied squares. "
- "name": "Cackletongue"
  "type": "Maneuver"
  "cost": "4 Malice"
  "keywords":
  - "--"
  "distance": "2 burst"
  "target": "All allies"
  "effects":
  - "name": "Effect"
    "effect": "1 [[Abyssal Hyena|abyssal hyena]] target turns into a [[Gnoll Marauder|gnoll marauder]], keeping their Stamina.\
      \ Targets who haven't used a cackletongue maneuver on this turn use it immediately\
      \ at no cost. "

```
