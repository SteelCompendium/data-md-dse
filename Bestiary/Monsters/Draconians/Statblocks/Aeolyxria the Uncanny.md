---
agility: 2
ancestry:
- Draconian
- Dragon
- Humanoid
ev: '32'
file_basename: Aeolyxria the Uncanny
file_dpath: Monsters/Draconians/Statblocks
free_strike: 7
intuition: 3
item_id: aeolyxria-the-uncanny
item_index: '104'
item_name: Aeolyxria the Uncanny
level: 6
might: -1
presence: 1
reason: 2
roles:
- Elite Controller
scc:
- mcdm.monsters.v1:monster:aeolyxria-the-uncanny
scdc:
- 1.1.1:2:104
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '140'
type: monster
---

~~~ds-statblock
type: statblock
name: Aeolyxria the Uncanny
level: 6
roles:
  - Elite Controller
ancestry:
  - Draconian
  - Dragon
  - Humanoid
ev: "32"
stamina: "140"
immunities:
  - Poison 6
speed: 5
movement: Fly
size: 1M
stability: 2
free_strike: 7
might: -1
agility: 2
reason: 2
intuition: 3
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Spittlesplash
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 10
    target: Two enemies
    effects:
      - roll: Power Roll + 3
        tier1: 10 poison damage; M < 1 slowed (save ends)
        tier2: 15 poison damage; M < 2 slowed (save ends)
        tier3: 18 poison damage; M < 3 slowed (save ends)
  - type: feature
    feature_type: ability
    name: Experimental Treasure
    icon: 🏹
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 10
    target: Two creature or objects
    effects:
      - roll: Power Roll + 3
        tier1: The targets regains 10 Stamina.
        tier2: 12 corruption damage; A < 2 weakened (save ends)
        tier3: 12 lightning damage; A < 2 bleeding (save ends)
      - name: Effect
        effect: The first time in an encounter that Aeolyxria makes a power roll for
          this ability, she can subsequently use the outcome of that roll
          instead of rolling whenever she uses this ability until the end of the
          encounter.
      - cost: 2+ Malice
        effect: The ability targets one additional target for each 2 Malice spent.
  - type: feature
    feature_type: ability
    name: Elevate
    icon: 🔳
    cost: 2 Malice
    keywords:
      - Area
      - Ranged
    usage: Maneuver
    distance: 1 cube within 5
    target: Special
    effects:
      - name: Effect
        effect: The ground in the area rises 5 squares, creating a pillar of dirt. Any
          creature in the area moves with the ground to its new elevation.
      - cost: 1+ Malice
        effect: Aeolyxria creates an additional pillar for each Malice spent.
  - type: feature
    feature_type: ability
    name: Blood For Blood
    icon: ❗️
    keywords:
      - Ranged
      - Weapon
    usage: Triggered action
    distance: Ranged 5
    target: One creature
    trigger: An ally is made bleeding by the target.
    effects:
      - roll: Power Roll + 3
        tier1: 7 poison damage; A < 2 bleeding (save ends)
        tier2: 12 poison damage; A < 3 bleeding (save ends)
        tier3: 15 poison damage; bleeding (save ends)
  - type: feature
    feature_type: trait
    name: That's Our Opening!
    icon: ⭐️
    effects:
      - effect: The Director gains 1 Malice whenever Aeolyxria imposes a condition on an
          enemy.
~~~