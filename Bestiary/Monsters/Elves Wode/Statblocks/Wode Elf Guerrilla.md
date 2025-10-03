---
agility: 2
ancestry:
- Fey
- Humanoid
- Wode Elf
ev: '10'
file_basename: Wode Elf Guerrilla
file_dpath: Monsters/Elves Wode/Statblocks
free_strike: 5
intuition: 0
item_id: wode-elf-guerrilla
item_index: '230'
item_name: Wode Elf Guerrilla
level: 3
might: 0
presence: 1
reason: 0
roles:
- Platoon Ambusher
scc:
- mcdm.monsters.v1:monster:wode-elf-guerrilla
scdc:
- 1.1.1:2:230
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '50'
type: monster
---

~~~ds-statblock
type: statblock
name: Wode Elf Guerrilla
level: 3
roles:
  - Platoon Ambusher
ancestry:
  - Fey
  - Humanoid
  - Wode Elf
ev: "10"
stamina: "50"
speed: 7
movement: Teleport
size: 1M
stability: 0
free_strike: 5
might: 0
agility: 2
reason: 0
intuition: 0
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Splinter Dagger
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Magic
      - Melee
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1 or ranged 5
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 7 damage
        tier2: 11 damage
        tier3: 14 damage; M < 2 bleeding (save ends)
      - name: Effect
        effect: The guerrilla can teleport up to 3 squares.
      - cost: 3 Malice
        effect: This ability targets one additional target, and deals an additional 3
          damage if both targets are adjacent to each other.
  - type: feature
    feature_type: ability
    name: Do Not Hesitate in the Wode
    icon: ❗️
    cost: 3 Malice
    keywords:
      - Ranged
    usage: Free triggered action
    distance: Ranged 20
    target: Self and each ally
    trigger: An ally ends their turn while the guerrilla hasn't acted this round.
    effects:
      - name: Special
        effect: The guerrilla must be acting as a captain.
      - name: Effect
        effect: The targets take their turn immediately. Each target gains an edge on
          abilities until the end of their turn.
  - type: feature
    feature_type: trait
    name: Into the Green
    icon: ⭐️
    effects:
      - effect: The guerrilla can attempt to hide at the end of each of their turns.
  - type: feature
    feature_type: trait
    name: Masking Glamor
    icon: ⭐️
    effects:
      - effect: Abilities targeting the guerrilla that would take a bane from cover or
          concealment have a double bane instead.
~~~