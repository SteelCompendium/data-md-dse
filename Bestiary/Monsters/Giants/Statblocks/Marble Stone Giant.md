---
agility: 3
ancestry:
- Giant
- Stone Giant
ev: '40'
file_basename: Marble Stone Giant
file_dpath: Monsters/Giants/Statblocks
free_strike: 8
intuition: 3
item_id: marble-stone-giant
item_index: '201'
item_name: Marble Stone Giant
level: 8
might: 4
presence: 0
reason: 0
roles:
- Elite Hexer
scc:
- mcdm.monsters.v1:monster:marble-stone-giant
scdc:
- 1.1.1:2:201
size: '4'
source: mcdm.monsters.v1
speed: 6
stability: 10
stamina: '207'
type: monster
---

~~~ds-statblock
type: statblock
name: Marble Stone Giant
level: 8
roles:
  - Elite Hexer
ancestry:
  - Giant
  - Stone Giant
ev: "40"
stamina: "207"
speed: 6
movement: Burrow
size: "4"
stability: 10
free_strike: 8
might: 4
agility: 3
reason: 0
intuition: 3
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Marble From a Great Sling
    icon: 🔳
    ability_type: Signature Ability
    keywords:
      - Area
      - Ranged
      - Weapon
    usage: Main action
    distance: 3 cube within 15
    target: Each enemy and object in the area
    effects:
      - roll: Power Roll + 4
        tier1: 6 damage; I < 2 dazed (save ends)
        tier2: 10 damage; I < 3 dazed (save ends)
        tier3: 14 damage; I < 4 dazed (save ends)
      - name: Effect
        effect: If the target has any effect on them that can be ended by a saving throw
          or that ends at the end of their turn, they are also knocked prone.
  - type: feature
    feature_type: ability
    name: Far Flung
    icon: 🗡
    cost: 3 Malice
    keywords:
      - Melee
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        tier1: Vertical push 7
        tier2: Vertical push 10
        tier3: Vertical push 12
      - name: Effect
        effect: Against a target who is prone or grabbed, this ability has a double
          edge.
  - type: feature
    feature_type: ability
    name: Polish Stone Shape
    icon: 🔳
    keywords:
      - Area
    usage: Maneuver
    distance: 10 x 2 line within 1
    target: Special
    effects:
      - name: Effect
        effect: The ground in the area becomes slick and glossy. Any non-giant who
          starts or ends their turn in the area is knocked prone and slides 2
          squares.
  - type: feature
    feature_type: ability
    name: Break Armor
    icon: ❗️
    cost: 1 Malice
    keywords:
      - "-"
    usage: Triggered action
    distance: Self
    target: Self
    trigger: The marble stone giant takes damage.
    effects:
      - name: Effect
        effect: The marble stone giant halves the damage, and has damage weakness 3 and
          a +3 bonus to speed until the end of the encounter. The damage
          weakness increases by 3 each time the marble stone giant uses this
          ability in the same encounter.
  - type: feature
    feature_type: trait
    name: Stonebreaker Flesh
    icon: ⭐️
    effects:
      - effect: Whenever an enemy obtains a tier 1 outcome on a melee ability used
          against the marble stone giant, they take a bane on that ability until
          the end of the encounter.
  - type: feature
    feature_type: trait
    name: Stone Steps
    icon: ⭐️
    effects:
      - effect: The marble stone giant ignores difficult terrain.
  - type: feature
    feature_type: trait
    name: Stone Swim
    icon: ⭐️
    effects:
      - effect: The marble stone giant can burrow through stone, but can't drag other
          creatures underground when they do so.
~~~