---
agility: 4
ancestry:
- Undead
ev: '9'
file_basename: Haunt
file_dpath: Monsters/Undead/Statblocks
free_strike: 3
intuition: 0
item_id: haunt
item_index: '62'
item_name: Haunt
level: 7
might: -2
presence: 0
reason: -1
roles:
- Horde Controller
scc:
- mcdm.monsters.v1:monster:haunt
scdc:
- 1.1.1:2:62
size: '2'
source: mcdm.monsters.v1
speed: 6
stability: 1
stamina: '40'
type: monster
---

~~~ds-statblock
type: statblock
name: Haunt
level: 7
roles:
  - Horde Controller
ancestry:
  - Undead
ev: "9"
stamina: "40"
immunities:
  - Corruption 7
  - poison 7
speed: 6
movement: Fly, hover
size: "2"
stability: 1
free_strike: 3
might: -2
agility: 4
reason: -1
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Lash Out
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 3
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        tier1: 7 damage; slide 2
        tier2: 10 damage; slide 3
        tier3: 11 damage; slide 5
      - name: Effect
        effect: If the target is force moved into another creature's space, that
          creature takes an additional 4 damage and the haunt slides them up to
          2 squares.
  - type: feature
    feature_type: ability
    name: Crushing Despair
    icon: ❇️
    cost: 3 Malice
    keywords:
      - Area
      - Magic
    usage: Main action
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        tier1: 3 damage; I < 2 prone
        tier2: 6 damage; I < 3 prone
        tier3: 7 damage; I < 4 prone
      - name: Effect
        effect: A target knocked prone this way can't use the Stand Up maneuver on
          themself while any haunt is within 20 squares of them.
  - type: feature
    feature_type: trait
    name: Invisible Horror
    icon: ⭐️
    effects:
      - effect: The haunt can move through creatures and objects at their usual speed,
          but can't end their turn inside a creature or object. They are
          invisible while moving using a move action. The haunt doesn't take
          damage from being force moved into objects.
~~~