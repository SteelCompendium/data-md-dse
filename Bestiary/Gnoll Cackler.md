```ds-statblock
"name": "Gnoll Cackler"
"ancestry":
- "Fiend"
- "Gnoll"
"roles":
- "Hexer"
"level": !!int "2"
"ev": !!int "11"
"stamina": !!int "20"
"immunities": []
"weaknesses": []
"speed": "5"
"size": "1S"
"stability": !!int "1"
"free_strike": !!int "3"
"might": !!int "0"
"intuition": !!int "2"
"agility": !!int "0"
"reason": !!int "2"
"presence": !!int "2"
"traits":
- "name": "Death Frenzy"
  "effect": "Whenever an ally within 5 is reduced to 0 Stamina, the cackler moves\
    \ up to their speed and takes a free strike."
"abilities":
- "name": "Moment of Brutality"
  "type": "Action"
  "cost": "Signature"
  "keywords":
  - "Magic"
  - "Ranged"
  - "Resistance"
  "distance": "Ranged 8"
  "target": "1 creature"
  "effects":
  - "roll": "2d10 + 2"
    "t1": "3 psychic damage; I1 target makes a free strike against a creature of the\
      \ cackler's choice"
    "t2": "5 psychic damage; I2 target makes a free strike against a creature of the\
      \ cackler's choice"
    "t3": "7 psychic damage; I3 target uses a signature ability against a creature\
      \ of the cackler's choice"
  - "name": "Effect"
    "effect": "An ally targeted by this ability makes a free strike instead of taking\
      \ damage. "
- "name": "Cackletongue"
  "type": "Maneuver"
  "cost": "4 Malice"
  "keywords":
  - "Area"
  - "Magic"
  - "Resistance"
  "distance": "2 burst"
  "target": "All creatures"
  "effects":
  - "roll": "INU RR"
    "t1": "Frightened of the cackler (save ends)"
    "t2": "Frightened of the cackler (EoT)"
    "t3": "No effect"
  - "name": "Effect"
    "effect": "Allies targeted by this ability don't make a resistance roll. Targets\
      \ who haven't used a cackletongue maneuver on this turn use it immediately at\
      \ no cost. "

```
