---
agility: 3
ancestry:
- Undead
ev: '144'
file_basename: Lich
file_dpath: Monsters/Lich/Statblocks
free_strike: 10
intuition: 5
item_id: lich
item_index: '349'
item_name: Lich
level: 10
might: 2
presence: 5
reason: 5
roles:
- Solo
scc:
- mcdm.monsters.v1:monster:lich
scdc:
- 1.1.1:2:349
size: 1M
source: mcdm.monsters.v1
speed: 10
stability: 1
stamina: '650'
type: monster
---

~~~ds-statblock
type: statblock
name: Lich
level: 10
roles:
  - Solo
ancestry:
  - Undead
ev: "144"
stamina: "650"
immunities:
  - Corruption 10
  - poison 10
weaknesses:
  - Holy 5
speed: 10
movement: Fly, hover
size: 1M
stability: 1
free_strike: 10
might: 2
agility: 3
reason: 5
intuition: 5
presence: 5
features:
  - type: feature
    feature_type: trait
    name: Solo Monster
    icon: ☠️
    effects:
      - name: End Effect
        effect: At the end of each of their turns, the lich can take 20 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
      - name: Solo Turns
        effect: The lich can take two turns each round. They can't take turns
          consecutively.
  - type: feature
    feature_type: ability
    name: Conflagration
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 20
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 5
        tier1: 15 fire damage; A < 4 the target is immolated (save ends)
        tier2: 21 fire damage; A < 5 the target is immolated (save ends)
        tier3: 25 fire damage; A < 6 the target is immolated (save ends)
      - name: Effect
        effect: An immolated creature takes 10 fire damage whenever they use a main
          action and a maneuver on their turn. This damage can't be reduced in
          any way.
  - type: feature
    feature_type: ability
    name: Hopeless Place
    icon: ❇️
    keywords:
      - Area
      - Magic
    usage: Main action
    distance: 10 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 5
        tier1: 8 corruption damage; P < 4 the target is hopeless (save ends)
        tier2: 13 corruption damage; P < 5 the target is hopeless (save ends)
        tier3: 16 corruption damage; P < 6 the target is hopeless (save ends)
      - name: Effect
        effect: A hopeless creature can't benefit from edges or double edges, can't gain
          or use surges, and can't gain temporary Stamina.
      - cost: 3 Malice
        effect: The distance of this ability increases to a 20 burst and its potency
          increases by 1.
  - type: feature
    feature_type: ability
    name: Pain Unending
    icon: 🏹
    cost: 2 Malice
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 20
    target: One creature or object
    effects:
      - roll: Power Roll + 5
        tier1: 17 psychic damage
        tier2: 24 psychic damage
        tier3: 29 psychic damage
      - name: Effect
        effect: A target who has M < 4 is wracked with pain (save ends). A creature
          wracked with pain has a double bane on abilities.
      - cost: 3 Malice
        effect: The lich chooses one additional target.
      - cost: 2+ Malice
        effect: "Each creature wracked with pain gains one of the following conditions
          of the lich's choice for each 2 Malice spent: bleeding, slowed, or
          prone and can't stand. These conditions end when a creature is no
          longer wracked with pain."
  - type: feature
    feature_type: ability
    name: Baleful Swap
    icon: ❗️
    cost: 2 Malice
    keywords:
      - Ranged
    usage: Triggered action
    distance: Ranged 10
    target: One enemy
    trigger: The lich is targeted using an ability by a creature other than the target.
    effects:
      - name: Effect
        effect: If the target has P < 4, they swap places with the lich to become the
          new target of the triggering ability.
  - type: feature
    feature_type: trait
    name: Herald of Oblivion
    icon: ⭐️
    effects:
      - effect: In the lich's presence, death's call is stronger. Any winded creature
          within 5 squares of the lich is bleeding and can't use the Catch
          Breath maneuver.
  - type: feature
    feature_type: trait
    name: Glare of Undeath
    icon: ⭐️
    effects:
      - effect: At the start of each round, the lich chooses a creature within 10
          squares. If that creature has R < 4, they are restrained until the end
          of the lich's next turn. The lich can't choose the same creature two
          rounds in a row.
  - type: feature
    feature_type: trait
    name: Rejuvenation
    icon: ⭐️
    effects:
      - effect: >-
          The lich has a soulstone, which has 50 Stamina and damage immunity all
          except to sonic damage and holy damage. If the lich is destroyed while
          their soulstone is intact, their soul retreats into the soulstone. Any
          creature who has P < 5 and who moves within 5 squares of an inhabited
          soulstone for the first time in a round or starts their turn there is
          compelled (save ends). A compelled creature must do everything in
          their power to move toward and touch the soulstone.


          A creature who touches an inhabited soulstone makes a **Might test**
          that takes a bane.
        tier1: The creature is reduced to 0 Stamina and the lich manifests adjacent to
          the soulstone with full Stamina.
        tier2: The creature is reduced to 0 Stamina and the lich manifests adjacent to
          the soulstone with 300 Stamina.
        tier3: The creature has their Stamina reduced to their winded value unless it is
          already lower, and the lich manifests adjacent to the soulstone with
          100 Stamina.
  - type: feature
    feature_type: ability
    name: Cages of Wasting
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
      - Magic
      - Ranged
    usage: "-"
    distance: Two 3 cubes within 10
    target: Each creature in the area
    effects:
      - name: Effect
        effect: Each target makes an Agility test.
        tier1: 10 corruption damage; restrained (save ends)
        tier2: 16 corruption damage; restrained (EoT)
        tier3: 20 corruption damage
      - name: Effect
        effect: The lich deals an additional 10 corruption damage to each creature
          restrained this way.
  - type: feature
    feature_type: ability
    name: My Power Alone
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - Area
      - Magic
    usage: "-"
    distance: 12 burst
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: A target can't use heroic abilities until the start of the lich's next
          turn.
  - type: feature
    feature_type: ability
    name: Arms of Necrosis
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Area
      - Magic
    usage: "-"
    distance: 6 burst
    target: Each creature in the area
    effects:
      - roll: Power Roll + 5
        tier1: 8 corruption damage; A < 4 frightened (save ends)
        tier2: 13 corruption damage; A < 5 frightened (save ends)
        tier3: 16 corruption damage; A < 6 frightened (save ends)
      - name: Effect
        effect: At the end of each of the lich's turns, they regain 10 Stamina for each
          creature frightened this way.
~~~