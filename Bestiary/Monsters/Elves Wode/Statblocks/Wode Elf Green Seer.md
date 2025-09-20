---
agility: 1
ancestry:
- Fey
- Humanoid
- Wode Elf
ev: '6'
file_basename: Wode Elf Green Seer
file_dpath: Monsters/Elves Wode/Statblocks
free_strike: 3
intuition: 2
item_id: wode-elf-green-seer
item_index: '223'
item_name: Wode Elf Green Seer
level: 1
might: 0
presence: 1
reason: 0
roles:
- Platoon Hexer
scc:
- mcdm.monsters.v1:monster:wode-elf-green-seer
scdc:
- 1.1.1:2:223
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '20'
type: monster
---

~~~ds-statblock
type: statblock
name: Wode Elf Green Seer
level: 1
roles:
  - Platoon Hexer
ancestry:
  - Fey
  - Humanoid
  - Wode Elf
ev: "6"
stamina: "20"
speed: 7
size: 1M
stability: 0
free_strike: 3
might: 0
agility: 1
reason: 0
intuition: 2
presence: 1
features:
  - type: feature
    feature_type: ability
    name: The Forest's Embrace
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 5 damage
        tier2: 7 damage; I < 1 restrained (save ends)
        tier3: 9 damage; I < 2 restrained (save ends)
      - name: Effect
        effect: While restrained this way, a target can't search for hidden creatures.
  - type: feature
    feature_type: ability
    name: The Natural Cycle
    icon: 🏹
    cost: 3 Malice
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Maneuver
    distance: Ranged 10
    target: Two creatures
    effects:
      - roll: Power Roll + 2
        tier1: 2 damage
        tier2: 4 damage; P < 1 weakened (save ends)
        tier3: 6 damage; P < 1 bleeding (save ends); the target has a double bane on
          strikes (save ends)
      - name: Effect
        effect: While bleeding or weakened this way, a target is covered in lichen.
  - type: feature
    feature_type: ability
    name: Foreseen Punishment
    icon: ❗️
    keywords:
      - Ranged
    usage: Free triggered action
    distance: Ranged 5
    target: The triggering creature
    trigger: A creature uses a triggered action targeting the green seer or an ally
      within distance.
    effects:
      - name: Effect
        effect: The green seer makes a free strike against the target after the target's
          triggered action is resolved.
  - type: feature
    feature_type: trait
    name: Masking Glamor
    icon: ⭐️
    effects:
      - effect: Abilities targeting the green seer that would take a bane from cover or
          concealment have a double bane instead.
~~~