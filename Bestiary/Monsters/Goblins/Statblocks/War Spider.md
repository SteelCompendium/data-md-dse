---
agility: 1
ancestry:
- Animal
- Goblin
ev: '12'
file_basename: War Spider
file_dpath: Monsters/Goblins/Statblocks
free_strike: 4
intuition: 0
item_id: war-spider
item_index: '312'
item_name: War Spider
level: 1
might: 2
presence: -3
reason: -4
roles:
- Elite Mount
scc:
- mcdm.monsters.v1:monster:war-spider
scdc:
- 1.1.1:2:312
size: '3'
source: mcdm.monsters.v1
speed: 7
stability: 2
stamina: '60'
type: monster
---

~~~ds-statblock
type: statblock
name: War Spider
level: 1
roles:
  - Elite Mount
ancestry:
  - Animal
  - Goblin
ev: "12"
stamina: "60"
speed: 7
movement: Climb
size: "3"
stability: 2
free_strike: 4
might: 2
agility: 1
reason: -4
intuition: 0
presence: -3
features:
  - type: feature
    feature_type: ability
    name: Bite
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature
    effects:
      - roll: Power Roll + 2
        tier1: 7 poison damage
        tier2: 11 poison damage
        tier3: 14 poison damage; M < 2 weakened (save ends)
      - cost: 2 Malice
        effect: For any tier outcome, if the target has M < 3, they are weakened (save
          ends).
  - type: feature
    feature_type: ability
    name: Leg Blade
    icon: 🗡
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        tier1: 6 damage
        tier2: 9 damage
        tier3: 12 damage
  - type: feature
    feature_type: ability
    name: Trample
    icon: 👤
    cost: 5 Malice
    keywords:
      - "-"
    usage: Main action
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The spider shifts up to their speed and uses Leg Blade against each
          creature who comes adjacent to them during the shift. The spider makes
          one power roll against all targets.
  - type: feature
    feature_type: ability
    name: Web
    icon: 🔳
    keywords:
      - Area
      - Weapon
    usage: Maneuver
    distance: 3 cube within 1
    target: Each creature in the area
    effects:
      - roll: Power Roll + 2
        tier1: A < 0 restrained (save ends)
        tier2: A < 1 restrained (save ends)
        tier3: A < 2 restrained (save ends)
      - name: Effect
        effect: The area is difficult terrain for enemies.
  - type: feature
    feature_type: ability
    name: Skitter
    icon: ❗️
    keywords:
      - "-"
    usage: Triggered action
    distance: Self
    target: Self
    trigger: The spider or any ally riding the spider takes damage.
    effects:
      - name: Effect
        effect: The damage is halved, and the spider shifts up to 2 squares after the
          triggering effect resolves.
  - type: feature
    feature_type: trait
    name: Ride Launcher
    icon: ⭐️
    effects:
      - effect: Any ally who leaps off the back of the spider can jump up to 6 squares
          without making a test, and takes no damage if they fall during the
          jump. After any ally jumps, the first melee strike the make on the
          same turn gains an edge.
  - type: feature
    feature_type: trait
    name: Wide Back
    icon: ⭐️
    effects:
      - effect: While riding the spider, two size 1 allies can occupy the same space.
~~~