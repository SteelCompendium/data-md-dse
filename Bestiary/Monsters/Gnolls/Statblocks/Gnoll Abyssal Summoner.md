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
type: statblock
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
features:
  - type: feature
    feature_type: ability
    name: Flame Wad
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 5
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 4 fire damage
        tier2: 5 fire damage
        tier3: 7 fire damage; I < 2 the target is burning (save ends)
      - name: Effect
        effect: A burning creature takes 1d6 fire damage at the start of each of their
          turns. A burning object takes 1d6 fire damage at the end of each
          round.
  - type: feature
    feature_type: ability
    name: Call Abyssal Hyenas
    icon: 🏹
    cost: 3 Malice
    keywords:
      - Ranged
    usage: Maneuver
    distance: Ranged 5
    target: Special
    effects:
      - name: Effect
        effect: Two abyssal hyenas claw up from the ground in unoccupied spaces within
          distance.
  - type: feature
    feature_type: ability
    name: Summoner's Cackletongue
    icon: ❇️
    cost: 4 Malice
    keywords:
      - Area
    usage: Maneuver
    distance: 2 burst
    target: Each ally in the area
    effects:
      - name: Effect
        effect: One abyssal hyena target turns into a gnoll marauder, keeping their
          current Stamina. If any target hasn't used their own Cackletongue
          maneuver on this turn, they can use it immediately at no cost.
  - type: feature
    feature_type: trait
    name: Death Frenzy
    icon: ⭐️
    effects:
      - effect: Whenever a non-minion ally within 5 squares of the abyssal summoner is
          reduced to 0 Stamina, the abyssal summoner moves up to their speed and
          can make a melee free strike.
~~~