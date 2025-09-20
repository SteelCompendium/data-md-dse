---
agility: 1
ancestry:
- Giant
- Ogre
ev: '16'
file_basename: Ogre Juggernaut
file_dpath: Monsters/Ogres/Statblocks
free_strike: 5
intuition: 0
item_id: ogre-juggernaut
item_index: '06'
item_name: Ogre Juggernaut
level: 2
might: 2
presence: -1
reason: -1
roles:
- Elite Harrier
scc:
- mcdm.monsters.v1:monster:ogre-juggernaut
scdc:
- 1.1.1:2:06
size: '2'
source: mcdm.monsters.v1
speed: 6
stability: 2
stamina: '80'
type: monster
---

~~~ds-statblock
type: statblock
name: Ogre Juggernaut
level: 2
roles:
  - Elite Harrier
ancestry:
  - Giant
  - Ogre
ev: "16"
stamina: "80"
speed: 6
size: "2"
stability: 2
free_strike: 5
might: 2
agility: 1
reason: -1
intuition: 0
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Pitchfork Catapult
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        tier1: 7 damage
        tier2: 10 damage; A < 1 vertical push 2
        tier3: 13 damage; A < 2 vertical slide 3
      - cost: 1 Malice
        effect: Each target who has M < 1 is bleeding (save ends).
  - type: feature
    feature_type: ability
    name: Earth-Breaking Jump
    icon: ❇️
    keywords:
      - Area
      - Weapon
    usage: Main action
    distance: 3 burst
    target: Each creature in the area
    effects:
      - name: Effect
        effect: The juggernaut jumps up to 6 squares before using this ability.
      - roll: Power Roll + 2
        tier1: 4 damage
        tier2: 6 damage; push 2; M < 1 prone
        tier3: 9 damage; push 4; M < 2 prone
  - type: feature
    feature_type: ability
    name: Horrible Bellow
    icon: ❇️
    cost: 2 Malice
    keywords:
      - Area
    usage: Maneuver
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        tier1: I < 0 frightened (save ends)
        tier2: I < 1 frightened (save ends)
        tier3: I < 2 frightened (save ends)
      - name: Effect
        effect: While a target is frightened this way, any ogre gains an edge on strikes
          against them.
  - type: feature
    feature_type: ability
    name: Hrraaaaaagh!
    icon: ❗️
    keywords:
      - "-"
    usage: Free triggered action
    distance: Self
    target: Self
    trigger: The juggernaut takes damage.
    effects:
      - name: Effect
        effect: The juggernaut moves up to their speed and can make a free strike.
  - type: feature
    feature_type: trait
    name: Destructive Path
    icon: ⭐️
    effects:
      - effect: The juggernaut automatically destroys any mundane size 1 objects in
          their path when they move or are forced moved. They can break through
          any mundane wall made of wood, stone, or a similarly sturdy material
          this way as long as the wall is 2 squares thick or less.
  - type: feature
    feature_type: trait
    name: Defiant Anger
    icon: ⭐️
    effects:
      - effect: While winded, the juggernaut has damage immunity 2.
~~~