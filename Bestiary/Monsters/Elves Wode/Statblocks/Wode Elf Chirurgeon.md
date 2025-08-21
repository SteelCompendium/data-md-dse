---
agility: 2
ancestry:
- Fey
- Humanoid
- Wode Elf
ev: '8'
file_basename: Wode Elf Chirurgeon
file_dpath: Monsters/Elves Wode/Statblocks
free_strike: 4
intuition: 0
item_id: wode-elf-chirurgeon
item_index: '235'
item_name: Wode Elf Chirurgeon
level: 2
might: 1
presence: 1
reason: 0
roles:
- Platoon Harrier
scc:
- mcdm.monsters.v1:monster:wode-elf-chirurgeon
scdc:
- 1.1.1:2:235
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '40'
type: monster
---

```ds-statblock
name: Wode Elf Chirurgeon
level: 2
roles:
  - Platoon Harrier
ancestry:
  - Fey
  - Humanoid
  - Wode Elf
ev: "8"
stamina: "40"
speed: 7
movement: Climb
size: 1M
stability: 0
free_strike: 4
might: 1
agility: 2
reason: 0
intuition: 0
presence: 1
traits:
  - name: Masking Glamor
    effects:
      - effect: Abilities targeting the chirurgeon that would take a bane from cover or
          concealment have a double bane instead.
abilities:
  - name: Wild Ax
    cost: Signature Ability
    keywords:
      - Charge
      - Melee
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1 or ranged 5
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 6 damage; push 1
        t2: 9 damage; push 3
        t3: 12 damage; push 5
      - effect: The chirurgeon can make a ranged free strike before using this ability.
        name: Effect
      - effect: The chirurgeon uses this ability again.
        cost: 5 Malice
  - name: The Wode Protects Us
    cost: 3 Malice
    keywords:
      - Magic
      - Ranged
    type: Maneuver
    distance: Ranged 5
    target: Self and three allies
    effects:
      - effect: Each target can teleport up to 10 squares to a space that has cover or
          concealment.
        name: Effect
```