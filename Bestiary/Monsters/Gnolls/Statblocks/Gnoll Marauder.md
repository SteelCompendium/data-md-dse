---
agility: 1
ancestry:
- Abyssal
- Gnoll
ev: '4'
file_basename: Gnoll Marauder
file_dpath: Monsters/Gnolls/Statblocks
free_strike: 2
intuition: 0
item_id: gnoll-marauder
item_index: '37'
item_name: Gnoll Marauder
level: 2
might: 1
presence: 1
reason: 0
roles:
- Horde Harrier
scc:
- mcdm.monsters.v1:monster:gnoll-marauder
scdc:
- 1.1.1:2:37
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 1
stamina: '20'
type: monster
---

```ds-statblock
name: Gnoll Marauder
level: 2
roles:
  - Horde Harrier
ancestry:
  - Abyssal
  - Gnoll
ev: "4"
stamina: "20"
speed: 7
size: 1M
stability: 1
free_strike: 2
might: 1
agility: 1
reason: 0
intuition: 0
presence: 1
traits:
  - name: Death Frenzy
    effects:
      - effect: Whenever a non-minion ally within 7 squares of the marauder is reduced
          to 0 Stamina, the marauder moves up to their speed and can make a
          melee free strike.
abilities:
  - name: Fury Flail
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 4 damage
        t2: 5 damage
        t3: 7 damage; prone; A < 2 bleeding (save ends)
      - effect: This ability targets one additional target for each 2 Malice spent.
        cost: 2+ Malice
  - name: Marauder's Cackletongue
    icon: ❇️
    cost: 3 Malice
    keywords:
      - Area
    type: Maneuver
    distance: 2 burst
    target: Self and each ally in the area
    effects:
      - effect: Each target shifts up to their speed. If any target hasn't used their
          own Cackletongue maneuver on this turn, they can use it immediately at
          no cost.
        name: Effect
```