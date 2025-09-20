---
agility: -1
ancestry:
- Giant
- Hill Giant
ev: '36'
file_basename: Hill Giant Clobberer
file_dpath: Monsters/Giants/Statblocks
free_strike: 8
intuition: -1
item_id: hill-giant-clobberer
item_index: '203'
item_name: Hill Giant Clobberer
level: 7
might: 4
presence: -1
reason: -1
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:hill-giant-clobberer
scdc:
- 1.1.1:2:203
size: '4'
source: mcdm.monsters.v1
speed: 6
stability: 5
stamina: '200'
type: monster
---

~~~ds-statblock
type: statblock
name: Hill Giant Clobberer
level: 7
roles:
  - Elite Brute
ancestry:
  - Giant
  - Hill Giant
ev: "36"
stamina: "200"
immunities:
  - Damage 3
speed: 6
movement: Climb
size: "4"
stability: 5
free_strike: 8
might: 4
agility: -1
reason: -1
intuition: -1
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Clobberin' Club
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 3
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        tier1: 12 damage
        tier2: 17 damage; prone
        tier3: 21 damage; prone
      - name: Effect
        effect: A target who is already prone takes an extra 12 damage.
  - type: feature
    feature_type: ability
    name: Stomp
    icon: 🗡
    cost: 3 Malice
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        tier1: 14 damage; prone
        tier2: 20 damage; prone; M < 3 can't stand (save ends)
        tier3: 25 damage; prone; M < 4 can't stand (save ends)
      - name: Effect
        effect: In suitably soft ground, the target is entrenched in a 2-square deep
          hole.
  - type: feature
    feature_type: ability
    name: Hill Quake
    icon: ❇️
    keywords:
      - Area
    usage: Maneuver
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: Each target must make either a **Might test** or an **Agility test**.
        tier1: 6 damage; vertical push 3
        tier2: 2 damage; vertical push 2
        tier3: Push 2
      - name: Effect
        effect: The clobberer can choose to fall prone in order to double the forced
          movement distance.
  - type: feature
    feature_type: ability
    name: You Ain't Getting Away
    icon: ❗️
    keywords:
      - Melee
    usage: Triggered action
    distance: Melee 3
    target: The triggering creature
    trigger: A creature within distance moves or shifts away from the clobberer.
    effects:
      - name: Effect
        effect: The target makes an Agility test.
        tier1: Grabbed, and the target takes a bane on the Escape Grab maneuver
        tier2: Grabbed
        tier3: No effect
      - cost: 2 Malice
        effect: A target who would be grabbed by this ability is instead either vertical
          pushed up to 5 squares; or they take 5 damage, are knocked prone, and
          can't stand until the end of their next turn.
  - type: feature
    feature_type: trait
    name: Destructive Path
    icon: ⭐️
    effects:
      - effect: The clobberer automatically destroys any mundane size 1 objects in their
          path when they move or are forced moved. They can break through any
          mundane wall made of wood, stone, or a similarly sturdy material this
          way as long as the wall is 2 squares thick or less.
  - type: feature
    feature_type: trait
    name: Distracted
    icon: ⭐️
    effects:
      - effect: Whenever the clobberer targets a creature or object with an ability, any
          enemy within distance of the ability can use a free triggered action
          to distract the clobberer. The clobberer targets that enemy instead.
~~~