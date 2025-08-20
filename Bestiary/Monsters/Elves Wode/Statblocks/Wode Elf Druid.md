---
agility: 1
ancestry:
- Fey
- Humanoid
- Wode Elf
ev: '8'
file_basename: Wode Elf Druid
file_dpath: Monsters/Elves Wode/Statblocks
free_strike: 3
intuition: 0
item_id: wode-elf-druid
item_index: '229'
item_name: Wode Elf Druid
level: 2
might: 0
presence: 2
reason: 0
roles:
- Platoon Controller
scc:
- mcdm.monsters.v1:monster:wode-elf-druid
scdc:
- 1.1.1:2:229
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '30'
type: monster
---

```ds-statblock
name: Wode Elf Druid
level: 2
roles:
  - Platoon Controller
ancestry:
  - Fey
  - Humanoid
  - Wode Elf
ev: "8"
stamina: "30"
speed: 7
movement: Climb
size: 1M
stability: 0
free_strike: 3
might: 0
agility: 1
reason: 0
intuition: 0
presence: 2
traits:
  - name: Masking Glamor
    effects:
      - effect: Abilities targeting the druid that would take a bane from cover or
          concealment have a double bane instead.
abilities:
  - name: Entangling Vines
    cost: Signature Ability
    keywords:
      - Area
      - Magic
      - Ranged
    type: Main action
    distance: 3 cube within 10
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        t1: 5 damage; pull 1
        t2: 8 damage; pull 3; M < 1 slowed (save ends)
        t3: 10 damage; pull 5; M < 2 slowed (save ends)
      - effect: While slowed this way, a target can't search for hidden creatures.
      - effect: The size of the cube and the potency both increase by 1.
        cost: 3 Malice
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
```