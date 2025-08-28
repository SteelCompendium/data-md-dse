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
traits:
  - name: Defiant Anger
    effects:
      - effect: While winded, the goon has damage immunity 2.
abilities:
  - name: Club Swing
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        t1: 7 damage; push 2
        t2: 11 damage; push 4
        t3: 14 damage; push 6, prone
      - effect: Any target who takes damage from this forced movement takes an extra 4
          damage.
        name: Effect
  - name: Grabby Hand
    icon: 🗡
    cost: 1 Malice
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Maneuver
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 7 damage
        t2: 11 damage; grabbed
        t3: 14 damage; grabbed
      - effect: A target grabbed this way takes a bane on the Escape Grab maneuver.
        name: Effect
  - name: People Bowling
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
      - Weapon
    type: Maneuver
    distance: 6 x 1 line within 1
    target: Each creature and object in the area
    effects:
      - name: Effect
        effect: The goon must have a size 1 creature or object grabbed, which they hurl
          across the area, ending the grab. The hurled creature or object is
          targeted by the ability, and lands in the last square of the line or
          the nearest unoccupied square of the goon's choice.
      - roll: Power Roll + 2
        t1: 5 damage
        t2: 9 damage
        t3: 12 damage; prone
  - name: Swat the Fly
    icon: ❗️
    keywords:
      - Melee
    type: Triggered action
    distance: Melee 1
    target: The triggering creature or object
    trigger: A creature or object within distance moves or shifts away from the goon.
    effects:
      - effect: The goon slides the target up to 5 squares
        name: Effect
~~~