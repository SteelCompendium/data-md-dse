---
agility: 1
ancestry:
- Beast
- Worm
ev: '108'
file_basename: Kingfissure Worm
file_dpath: Monsters/Kingfissure Worm/Statblocks
free_strike: 8
intuition: 2
item_id: kingfissure-worm
item_index: '245'
item_name: Kingfissure Worm
level: 7
might: 5
presence: -3
reason: -5
roles:
- Solo
scc:
- mcdm.monsters.v1:monster:kingfissure-worm
scdc:
- 1.1.1:2:245
size: '5'
source: mcdm.monsters.v1
speed: 10
stability: 5
stamina: '420'
type: monster
---

~~~ds-statblock
type: statblock
name: Kingfissure Worm
level: 7
roles:
  - Solo
ancestry:
  - Beast
  - Worm
ev: "108"
stamina: "420"
speed: 10
movement: Burrow
size: "5"
stability: 5
free_strike: 8
might: 5
agility: 1
reason: -5
intuition: 2
presence: -3
features:
  - type: feature
    feature_type: trait
    name: Solo Monster
    icon: ☠️
    effects:
      - name: End Effect
        effect: At the end of each of their turns, the kingfissure worm can take 10
          damage to end one effect on them that can be ended by a saving throw.
          This damage can't be reduced in any way.
      - name: Solo Turns
        effect: The kingfissure worm can take two turns each round. They can't take
          turns consecutively.
  - type: feature
    feature_type: trait
    name: Multiple Tongues
    icon: ⭐️
    effects:
      - effect: The kingfissure worm has three tongues. Each tongue is a 5 x 1 line
          within 1 square of the kingfissure worm, has 35 Stamina and psychic
          immunity all, and can't be force moved. Each tongue enables the
          kingfissure worm to grab one size 3 or smaller creature or object. A
          tongue can be targeted by abilities only while it has a target
          grabbed.
  - type: feature
    feature_type: ability
    name: Tongue Grab
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 5
    target: One creature or object per tongue
    effects:
      - roll: Power Roll + 5
        tier1: 13 damage; M < 3 grabbed
        tier2: 18 damage; M < 4 grabbed
        tier3: 22 damage; M < 5 grabbed and the target takes a bane on the Escape Grab
          maneuver
      - name: Effect
        effect: The kingfissure worm must have one or more tongues to use this ability.
          As a maneuver, the kingfissure worm can pull up to two creatures
          grabbed this way adjacent to them.
  - type: feature
    feature_type: ability
    name: Maw
    icon: 🗡
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 5
        tier1: 15 damage; push 3
        tier2: 20 damage; push 5, prone
        tier3: 25 damage; the target is swallowed (see Swallowed)
      - cost: 2 Malice
        effect: When the kingfissure worm uses the Charge main action, they ignore
          difficult terrain and automatically destroy mundane size 3 and smaller
          objects in the path of their charge. The first time the kingfissure
          worm moves through a creature's space during this charge, that
          creature takes 8 damage and is pushed up to 3 squares.
  - type: feature
    feature_type: ability
    name: Consume
    icon: 🗡
    cost: 2 Malice
    keywords:
      - Melee
    usage: Main action
    distance: Melee 1
    target: One grabbed creature
    effects:
      - name: Effect
        effect: The target is swallowed (see Swallowed).
  - type: feature
    feature_type: ability
    name: Tongue Whip
    icon: ⚔️
    keywords:
      - Melee
      - Ranged
      - Strike
      - Weapon
    usage: Maneuver
    distance: Melee 5 or ranged 10
    target: One creature or object
    effects:
      - name: Effect
        effect: The kingfissure worm can use this maneuver only while they have a
          creature or object grabbed. The worm slams the grabbed creature or
          object against the target, dealing 13 damage to both. If this ability
          is used at range, it deals an extra 5 damage and the grabbed creature
          or object is released.
  - type: feature
    feature_type: ability
    name: Tearing Recoil
    icon: ❗️
    keywords:
      - "-"
    usage: Triggered action
    distance: Self
    target: Special
    trigger: A tongue takes damage that doesn't reduce it to 0 Stamina.
    effects:
      - name: Effect
        effect: The kingfissure worm deals 5 damage to the creature or object the tongue
          had grabbed, releases that creature or object, then pulls the damaged
          tongue back into their mouth.
  - type: feature
    feature_type: trait
    name: Seismic King
    icon: ⭐️
    effects:
      - effect: The kingfissure worm has line of effect only within 3 squares However,
          they ignore concealment for creatures touching the ground and don't
          need line of effect to use abilities against those creatures.
  - type: feature
    feature_type: trait
    name: Swallowed
    icon: ⭐️
    effects:
      - effect: A creature swallowed by the kingfissure worm is restrained and takes 1d6
          acid damage at the start of every turn. If the worm takes 25 or more
          damage in a single round from swallowed creatures, they immediately
          regurgitate all creatures they have swallowed, who land prone in
          unoccupied spaces within 3 squares of the kingfissure worm.
  - type: feature
    feature_type: trait
    name: Titanic Tunneler
    icon: ⭐️
    effects:
      - effect: The kingfissure worm can burrow through stone. When the worm burrows,
          they create a stable size 3 tunnel in the squares they move through.
  - type: feature
    feature_type: trait
    name: Unstoppable Crawler
    icon: ⭐️
    effects:
      - effect: The kingfissure worm can't be frightened or knocked prone. While the
          worm is restrained or slowed, they take a −2 penalty to speed instead
          of suffering those conditions' usual effects on speed.
  - type: feature
    feature_type: ability
    name: King's Fissure
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
      - Weapon
    usage: "-"
    distance: 20 x 4 line within 1
    target: Each creature and object in the area
    effects:
      - name: Special
        effect: Each target must be on the ground.
      - name: Effect
        effect: The area becomes a 10-square-deep fissure in the earth. Each target
          makes an **Agility test**.
        tier1: 10 damage; the target falls into the fissure, lands prone, and can't
          stand (EoT)
        tier2: 10 damage; the target is knocked prone and left hanging at the edge of
          the area
        tier3: The target shifts to the nearest unoccupied space outside the area.
  - type: feature
    feature_type: ability
    name: Earth Breach
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - Weapon
    usage: "-"
    distance: Self
    target: Special
    effects:
      - name: Effect
        effect: The kingfissure worm can use this villain action only while burrowing.
          The worm burrows up to half their speed, then breaches the surface and
          moves 5 squares straight up before dropping back to the ground. Each
          creature or object whose space the worm moves through during this
          movement takes 10 damage, and if they have A < 4 they are knocked
          prone. Any creature who is made winded by this damage is swallowed
          (see Swallowed).
  - type: feature
    feature_type: ability
    name: Better Out Than In
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Area
      - Weapon
    usage: "-"
    distance: 5 burst
    target: Each enemy and object in the area
    effects:
      - roll: Power Roll + 5
        tier1: 8 acid damage; P < 3 weakened (save ends)
        tier2: 13 acid damage; P < 4 weakened (save ends)
        tier3: 17 acid damage; P < 5 weakened (save ends)
      - name: Effect
        effect: Each creature swallowed by the worm is regurgitated and automatically
          subject to the tier 3 outcome, then lands prone in an unoccupied space
          within 5 squares of the kingfissure worm.
~~~