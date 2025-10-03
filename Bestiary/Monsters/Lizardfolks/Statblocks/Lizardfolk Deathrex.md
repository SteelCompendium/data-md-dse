---
agility: 2
ancestry:
- Humanoid
- Lizardfolk
ev: '12'
file_basename: Lizardfolk Deathrex
file_dpath: Monsters/Lizardfolks/Statblocks
free_strike: 4
intuition: 1
item_id: lizardfolk-deathrex
item_index: '46'
item_name: Lizardfolk Deathrex
level: 1
might: 3
presence: 2
reason: 0
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:lizardfolk-deathrex
scdc:
- 1.1.1:2:46
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '80'
type: monster
---

~~~ds-statblock
type: statblock
name: Lizardfolk Deathrex
level: 1
roles:
  - Leader
ancestry:
  - Humanoid
  - Lizardfolk
ev: "12"
stamina: "80"
speed: 5
movement: Climb, swim
size: "2"
stability: 2
free_strike: 4
might: 3
agility: 2
reason: 0
intuition: 1
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Ripper Spear
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 3
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        tier1: 7 damage; pull 1; A < 1 bleeding (save ends)
        tier2: 10 damage; pull 1; A < 2 bleeding (save ends)
        tier3: 12 damage; pull 2; A < 3 bleeding (save ends)
      - cost: 1 Malice
        effect: One target adjacent to the deathrex is grabbed in the deathrex's mouth.
  - type: feature
    feature_type: ability
    name: Death Roll
    icon: 🗡
    cost: 3 Malice
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One grabbed creature or object
    effects:
      - roll: Power Roll + 3
        tier1: 8 damage; M < 1 dazed (save ends)
        tier2: 12 damage; M < 2 dazed (save ends)
        tier3: 15 damage; M < 3 dazed (save ends)
      - name: Effect
        effect: The target is no longer grabbed by the deathrex, and the deathrex slides
          them up to 5 squares.
  - type: feature
    feature_type: ability
    name: Trundle
    icon: 👤
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The deathrex moves up to their speed. They can make a free strike
          against each creature who makes an opportunity attack against them
          during this movement.
  - type: feature
    feature_type: ability
    name: Swat the Fly
    icon: ❗️
    keywords:
      - Melee
    usage: Triggered action
    distance: Melee 1
    target: The triggering creature or object
    trigger: A creature or object within distance moves or shifts away from the
      deathrex.
    effects:
      - name: Effect
        effect: The deathrex slides the target up to 5 squares.
  - type: feature
    feature_type: trait
    name: Rex Reptilian Escape
    icon: ⭐️
    effects:
      - effect: While the deathrex has a tail, whenever they are affected by an effect
          that can be ended by a saving throw or that ends at the end of their
          turn, they can lose their tail to immediately end that effect, then
          shift up to 2 squares.
  - type: feature
    feature_type: ability
    name: Snack Attack
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
    usage: "-"
    distance: 10 burst
    target: Self and each ally in the area
    effects:
      - name: Effect
        effect: Each target moves up to their speed and can make a free strike. Each
          target gains temporary Stamina equal to the damage they deal.
  - type: feature
    feature_type: ability
    name: Shed Some Skin
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - "-"
    usage: "-"
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The deathrex shifts up to their speed, leaving behind a shed skin
          duplicate in the space they started in. The duplicate acts on the
          deathrex's turn and has the deathrex's characteristics, but has 10
          Stamina and no villain actions.
  - type: feature
    feature_type: ability
    name: Thresher Thrasher
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Area
    usage: "-"
    distance: 10 burst
    target: Self and each ally in the area
    effects:
      - name: Effect
        effect: Each target moves up to their speed. Until the end of the encounter,
          whenever a creature comes adjacent to a target or starts their turn
          there, the target can make a free strike against them.
~~~