---
agility: 0
ancestry:
- Abyssal
- Gnoll
ev: '4'
file_basename: Gnoll Abyssal Summoner
file_dpath: Monsters/Gnolls/Statblocks
free_strike: 2
intuition: 2
item_id: gnoll-abyssal-summoner
item_index: '36'
item_name: Gnoll Abyssal Summoner
level: 2
might: 1
presence: 2
reason: 0
roles:
- Horde Support
scc:
- mcdm.monsters.v1:monster:gnoll-abyssal-summoner
scdc:
- 1.1.1:2:36
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '20'
type: monster
---

~~~ds-statblock
name: Gnoll Abyssal Summoner
level: 2
roles:
  - Horde Support
ancestry:
  - Abyssal
  - Gnoll
ev: "4"
stamina: "20"
speed: 5
size: 1M
stability: 1
free_strike: 2
might: 1
agility: 0
reason: 0
intuition: 2
presence: 2
traits:
  - name: Death Frenzy
    effects:
      - effect: Whenever a non-minion ally within 5 squares of the abyssal summoner is
          reduced to 0 Stamina, the abyssal summoner moves up to their speed and
          can make a melee free strike.
abilities:
  - name: Flame Wad
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 5
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 4 fire damage
        t2: 5 fire damage
        t3: 7 fire damage; I < 2 the target is burning (save ends)
      - effect: A burning creature takes 1d6 fire damage at the start of each of their
          turns. A burning object takes 1d6 fire damage at the end of each
          round.
        name: Effect
  - name: Call Abyssal Hyenas
    icon: 🏹
    cost: 3 Malice
    keywords:
      - Ranged
    type: Maneuver
    distance: Ranged 5
    target: Special
    effects:
      - effect: Two abyssal hyenas claw up from the ground in unoccupied spaces within
          distance.
        name: Effect
  - name: Summoner's Cackletongue
    icon: ❇️
    cost: 4 Malice
    keywords:
      - Area
    type: Maneuver
    distance: 2 burst
    target: Each ally in the area
    effects:
      - effect: One abyssal hyena target turns into a gnoll marauder, keeping their
          current Stamina. If any target hasn't used their own Cackletongue
          maneuver on this turn, they can use it immediately at no cost.
        name: Effect
~~~