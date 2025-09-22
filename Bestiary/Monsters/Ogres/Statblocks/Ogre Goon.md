---
agility: 0
ancestry:
- Giant
- Ogre
ev: '16'
file_basename: Ogre Goon
file_dpath: Monsters/Ogres/Statblocks
free_strike: 5
intuition: 0
item_id: ogre-goon
item_index: '02'
item_name: Ogre Goon
level: 2
might: 2
presence: -1
reason: -1
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:ogre-goon
scdc:
- 1.1.1:2:02
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 4
stamina: '100'
type: monster
---

~~~ds-statblock
type: statblock
name: Ogre Goon
level: 2
roles:
  - Elite Brute
ancestry:
  - Giant
  - Ogre
ev: "16"
stamina: "100"
speed: 5
size: "2"
stability: 4
free_strike: 5
might: 2
agility: 0
reason: -1
intuition: 0
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Club Swing
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
        tier1: 7 damage; push 2
        tier2: 11 damage; push 4
        tier3: 14 damage; push 6, prone
      - name: Effect
        effect: Any target who takes damage from this forced movement takes an extra 4
          damage.
  - type: feature
    feature_type: ability
    name: Grabby Hand
    icon: 🗡
    cost: 1 Malice
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Maneuver
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 7 damage
        tier2: 11 damage; grabbed
        tier3: 14 damage; grabbed
      - name: Effect
        effect: A target grabbed this way takes a bane on the Escape Grab maneuver.
  - type: feature
    feature_type: ability
    name: People Bowling
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
      - Weapon
    usage: Maneuver
    distance: 6 x 1 line within 1
    target: Each creature and object in the area
    effects:
      - name: Effect
        effect: The goon must have a size 1 creature or object grabbed, which they hurl
          across the area, ending the grab. The hurled creature or object is
          targeted by the ability, and lands in the last square of the line or
          the nearest unoccupied square of the goon's choice.
      - roll: Power Roll + 2
        tier1: 5 damage
        tier2: 9 damage
        tier3: 12 damage; prone
  - type: feature
    feature_type: ability
    name: Swat the Fly
    icon: ❗️
    keywords:
      - Melee
    usage: Triggered action
    distance: Melee 1
    target: The triggering creature or object
    trigger: A creature or object within distance moves or shifts away from the goon.
    effects:
      - name: Effect
        effect: The goon slides the target up to 5 squares.
  - type: feature
    feature_type: trait
    name: Defiant Anger
    icon: ⭐️
    effects:
      - effect: While winded, the goon has damage immunity 2.
~~~