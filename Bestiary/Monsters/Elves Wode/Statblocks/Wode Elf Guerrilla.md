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
item_index: '232'
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
- 1.1.1:2:232
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '50'
type: monster
---

```ds-statblock
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
traits:
  - name: Into the Green
    effects:
      - effect: The guerrilla can attempt to hide at the end of each of their turns.
  - name: Masking Glamor
    effects:
      - effect: Abilities targeting the guerrilla that would take a bane from cover or
          concealment have a double bane instead.
abilities:
  - name: Splinter Dagger
    icon: ⚔️
    cost: Signature Ability
    keywords:
      - Magic
      - Melee
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1 or ranged 5
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 7 damage
        t2: 11 damage
        t3: 14 damage; M < 2 bleeding (save ends)
      - effect: The guerrilla can teleport up to 3 squares.
        name: Effect
      - effect: This ability targets one additional target, and deals an additional 3
          damage if both targets are adjacent to each other.
        cost: 3 Malice
  - name: Do Not Hesitate in the Wode
    icon: ❗️
    cost: 3 Malice
    keywords:
      - Ranged
    type: Free triggered action
    distance: Ranged 20
    target: Self and each ally
    trigger: An ally ends their turn while the guerrilla hasn't acted this round.
    effects:
      - effect: The guerrilla must be acting as a captain.
        name: Special
      - effect: The targets take their turn immediately. Each target gains an edge on
          abilities until the end of their turn.
        name: Effect
```