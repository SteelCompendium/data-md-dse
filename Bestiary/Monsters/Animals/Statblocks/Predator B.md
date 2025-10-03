---
agility: 1
ancestry:
- Animal
ev: '16'
file_basename: Predator B
file_dpath: Monsters/Animals/Statblocks
free_strike: 5
intuition: 1
item_id: predator-b
item_index: '246'
item_name: Predator B
level: 3
might: 2
presence: 0
reason: -1
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:predator-b
scdc:
- 1.1.1:2:246
size: '3'
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '100'
type: monster
---

~~~ds-statblock
type: statblock
name: Predator B
level: 3
roles:
  - Elite Brute
ancestry:
  - Animal
ev: "16"
stamina: "100"
speed: 5
size: "3"
stability: 2
free_strike: 5
might: 2
agility: 1
reason: -1
intuition: 1
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Natural Weapon
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        tier1: 7 damage
        tier2: 11 damage; push 1; M < 1 prone
        tier3: 14 damage; push 2; M < 1 prone
  - type: feature
    feature_type: ability
    name: Wild Swing
    icon: ❇️
    keywords:
      - Area
      - Weapon
    usage: Main action
    distance: 1 burst
    target: Each enemy or object in the area
    effects:
      - roll: Power Roll + 2
        tier1: 3 damage
        tier2: 6 damage
        tier3: 8 damage; A < 2 bleeding (save ends)
  - type: feature
    feature_type: ability
    name: Swat
    icon: ❗️
    keywords:
      - Melee
    usage: Triggered action
    distance: Melee 1
    target: The triggering creature or object
    trigger: A creature or object within distance deals damage to the predator.
    effects:
      - name: Effect
        effect: The target is pushed up to 5 squares.
  - type: feature
    feature_type: trait
    name: Trample
    icon: ⭐️
    effects:
      - effect: The predator can move through enemies' and objects' spaces at their
          usual speed. Any mundane size 2 or smaller object whose space they
          move through is destroyed. When the predator enters a creature's space
          for the first time on a turn, that creature takes 3 damage.
  - type: feature
    feature_type: trait
    name: Nature's Spirit
    icon: ⭐️
    effects:
      - effect: While outdoors or in a natural environment, the predator can negate a
          bane on their abilities or turn a double bane into a bane.
~~~