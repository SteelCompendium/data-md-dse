---
agility: 1
ancestry:
- Humanoid
- Kobold
ev: '3'
file_basename: Kobold Legionary
file_dpath: Monsters/Kobolds/Statblocks
free_strike: 1
intuition: 0
item_id: kobold-legionary
item_index: '98'
item_name: Kobold Legionary
level: 1
might: 2
presence: 0
reason: 0
roles:
- Horde Defender
scc:
- mcdm.monsters.v1:monster:kobold-legionary
scdc:
- 1.1.1:2:98
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '20'
type: monster
---

~~~ds-statblock
type: statblock
name: Kobold Legionary
level: 1
roles:
  - Horde Defender
ancestry:
  - Humanoid
  - Kobold
ev: "3"
stamina: "20"
speed: 5
size: 1S
stability: 0
free_strike: 1
might: 2
agility: 1
reason: 0
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Gladius
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 5
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 3 damage; taunted (EoT)
        tier2: 4 damage; taunted (EoT)
        tier3: 5 damage; taunted (EoT)
      - cost: 3 Malice
        effect: If the legionary is acting as a captain, they and each member of their
          squad shift up to 2 squares before this ability is used.
  - type: feature
    feature_type: ability
    name: Shield Bash
    icon: 🗡
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Maneuver
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 2 damage; push 1; M < 0 prone
        tier2: 3 damage; push 1; M < 1 prone
        tier3: 4 damage; push 1; M < 2 prone
  - type: feature
    feature_type: trait
    name: Shield? Shield!
    icon: ⭐️
    effects:
      - effect: While adjacent to an ally who also has this trait, the legionary has
          stability 1, has cover, and grants cover to allies.
~~~