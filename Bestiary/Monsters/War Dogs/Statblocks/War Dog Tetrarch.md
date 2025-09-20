---
agility: 3
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '32'
file_basename: War Dog Tetrarch
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 7
intuition: 3
item_id: war-dog-tetrarch
item_index: '363'
item_name: War Dog Tetrarch
level: 6
might: 4
presence: 4
reason: 2
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:war-dog-tetrarch
scdc:
- 1.1.1:2:363
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 2
stamina: '180'
type: monster
---

~~~ds-statblock
type: statblock
name: War Dog Tetrarch
level: 6
roles:
  - Leader
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "32"
stamina: "180"
speed: 7
size: 1M
stability: 2
free_strike: 7
might: 4
agility: 3
reason: 2
intuition: 3
presence: 4
features:
  - type: feature
    feature_type: ability
    name: Houndblade
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Charge
      - Melee
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1 or ranged 3
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        tier1: 11 damage
        tier2: 16 damage; taunted (EoT)
        tier3: 19 damage; taunted (EoT)
      - name: Effect
        effect: A creature taunted this way takes a bane on strikes.
      - cost: 3 Malice
        effect: Each target loses 1d3 Recoveries.
  - type: feature
    feature_type: ability
    name: Get Them, You Dolts! 1 Malice per target
    icon: 🏹
    keywords:
      - Ranged
    usage: Maneuver
    distance: Ranged 10
    target: Three creatures
    effects:
      - name: Effect
        effect: Each target shifts up to their speed and can make a free strike. If the
          free strike targets an enemy taunted by the tetrarch, it deals an
          extra 4 damage.
  - type: feature
    feature_type: ability
    name: Sneering Disregard
    icon: ❗️
    keywords:
      - Ranged
    usage: Triggered action
    distance: Ranged 10
    target: The triggering creature
    trigger: A creature within distance who is not taunted by the tetrarch targets
      the tetrarch with a power roll.
    effects:
      - name: Effect
        effect: The power roll has a double bane. If the target obtains a tier 1
          outcome, the tetrarch ignores any of the power roll's effects other
          than damage and the target is frightened of the tetrarch (save ends).
  - type: feature
    feature_type: trait
    name: End Effect
    icon: ⭐️
    effects:
      - effect: At the end of each of their turns, the tetrarch can take 10 damage to
          end one effect on them that can be ended by a saving throw. This
          damage can't be reduced in any way.
  - type: feature
    feature_type: ability
    name: Enter the Fray
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
    usage: "-"
    distance: 2 burst
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: The tetrarch can jump up to 7 squares before using this ability.
      - roll: Power Roll + 4
        tier1: Push 2; I < 2 frightened (save ends)
        tier2: Push 4; I < 3 frightened (save ends)
        tier3: Push 5; I < 4 frightened (save ends)
  - type: feature
    feature_type: ability
    name: Lay Waste
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - Area
      - Ranged
      - Weapon
    usage: "-"
    distance: Five 2 cubes within 20
    target: Each creature and object in the area
    effects:
      - roll: Power Roll + 4
        tier1: 7 fire damage; A < 2 slowed (EoT)
        tier2: 13 fire damage; A < 3 slowed (save ends)
        tier3: 16 fire damage; A < 4 slowed (save ends)
      - name: Effect
        effect: The area is set ablaze until the end of the encounter. While ablaze, the
          area is difficult terrain, and any creature takes 2 fire damage for
          each square in the area they enter for the first time in a round
  - type: feature
    feature_type: ability
    name: You Would Dare?!
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - "-"
    usage: "-"
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: Until the end of the encounter, the tetrarch has damage immunity 2, and
          their Houndblade ability targets three creatures or objects.
~~~