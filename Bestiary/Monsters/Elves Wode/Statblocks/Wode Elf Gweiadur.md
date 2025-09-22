---
agility: 2
ancestry:
- Fey
- Humanoid
- Wode Elf
ev: '10'
file_basename: Wode Elf Gweiadur
file_dpath: Monsters/Elves Wode/Statblocks
free_strike: 5
intuition: 1
item_id: wode-elf-gweiadur
item_index: '228'
item_name: Wode Elf Gweiadur
level: 3
might: 0
presence: 0
reason: 0
roles:
- Platoon Artillery
scc:
- mcdm.monsters.v1:monster:wode-elf-gweiadur
scdc:
- 1.1.1:2:228
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '40'
type: monster
---

~~~ds-statblock
type: statblock
name: Wode Elf Gweiadur
level: 3
roles:
  - Platoon Artillery
ancestry:
  - Fey
  - Humanoid
  - Wode Elf
ev: "10"
stamina: "40"
speed: 7
movement: Climb
size: 1M
stability: 0
free_strike: 5
might: 0
agility: 2
reason: 0
intuition: 1
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Snare Bow
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 15
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 7 damage
        tier2: 11 damage
        tier3: 14 damage; A < 2 restrained (save ends)
      - name: Effect
        effect: The gweiadur shifts up to 3 squares.
      - cost: 3 Malice
        effect: If this ability restrains the target, one enemy adjacent to the target
          is also restrained (save ends).
  - type: feature
    feature_type: ability
    name: You Activated My Trap!
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    usage: Maneuver
    distance: 3 cube within 10
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        tier1: 4 damage; R < 0 the target is marked (save ends)
        tier2: 6 damage; R < 1 slowed and the target is marked (save ends)
        tier3: 9 damage; R < 2 slowed and the target is marked (save ends)
      - name: Effect
        effect: Allies gain an edge on abilities against a target marked by any wode
          elf.
  - type: feature
    feature_type: trait
    name: Masking Glamor
    icon: ⭐️
    effects:
      - effect: Abilities targeting the gweiadur that would take a bane from cover or
          concealment have a double bane instead.
~~~