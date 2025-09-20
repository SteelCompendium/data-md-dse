---
agility: 2
ancestry:
- Undead
- Soulless
ev: 3 for four minions
file_basename: Crawling Claw
file_dpath: Monsters/Undead/Statblocks
free_strike: 1
intuition: -1
item_id: crawling-claw
item_index: '75'
item_name: Crawling Claw
level: 1
might: 0
presence: -1
reason: -5
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster:crawling-claw
scdc:
- 1.1.1:2:75
size: 1T
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '4'
type: monster
---

~~~ds-statblock
type: statblock
name: Crawling Claw
level: 1
roles:
  - Minion Harrier
ancestry:
  - Undead
  - Soulless
ev: 3 for four minions
stamina: "4"
immunities:
  - Corruption 1
  - poison 1
speed: 6
movement: Climb
size: 1T
stability: 0
free_strike: 1
with_captain: +2 bonus to speed
might: 0
agility: 2
reason: -5
intuition: -1
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Fingernails
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 1 damage
        tier2: 2 damage
        tier3: 3 damage
      - name: Effect
        effect: The crawling claw shifts up to a number of squares equal to the damage
          dealt.
  - type: feature
    feature_type: trait
    name: Disorganized
    icon: ⭐️
    effects:
      - effect: Allies can't flank with the crawling cla.
~~~