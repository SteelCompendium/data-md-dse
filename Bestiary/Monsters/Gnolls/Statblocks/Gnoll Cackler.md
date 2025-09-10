---
agility: 0
ancestry:
- Abyssal
- Gnoll
ev: '4'
file_basename: Gnoll Cackler
file_dpath: Monsters/Gnolls/Statblocks
free_strike: 2
intuition: 2
item_id: gnoll-cackler
item_index: '41'
item_name: Gnoll Cackler
level: 2
might: 0
presence: 2
reason: 2
roles:
- Horde Hexer
scc:
- mcdm.monsters.v1:monster:gnoll-cackler
scdc:
- 1.1.1:2:41
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '15'
type: monster
---

~~~ds-statblock
name: Gnoll Cackler
level: 2
roles:
  - Horde Hexer
ancestry:
  - Abyssal
  - Gnoll
ev: "4"
stamina: "15"
speed: 5
size: 1S
stability: 1
free_strike: 2
might: 0
agility: 0
reason: 2
intuition: 2
presence: 2
traits:
  - name: Death Frenzy
    effects:
      - effect: Whenever a non-minion ally within 5 squares of the cackler is reduced to
          0 Stamina, the cackler moves up to their speed and can make a melee
          free strike.
abilities:
  - name: Moment of Brutality
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 8
    target: One creature
    effects:
      - roll: Power Roll + 2
        t1: 4 psychic damage; I < 0 the target makes a free strike against a creature of
          the cackler's choice
        t2: 5 psychic damage; I < 1 the target makes a free strike against a creature of
          the cackler's choice
        t3: 7 psychic damage; I < 2 the target uses a signature ability against a
          creature of the cackler's choice
      - effect: An ally targeted by this ability ignores the damage and can make a free
          strike.
        name: Effect
  - name: Cackler's Cackletongue
    icon: ❇️
    cost: 4 Malice
    keywords:
      - Area
      - Magic
    type: Maneuver
    distance: 2 burst
    target: Each creature in the area
    effects:
      - name: Effect
        effect: Each enemy target makes an **Intuition test**. If any target hasn't used
          their own Cackletongue maneuver on this turn, they can use it
          immediately at no cost.
        t1: Frightened (save ends)
        t2: Frightened (EoT)
        t3: No effect
~~~