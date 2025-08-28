---
agility: 2
ancestry:
- Fey
- Humanoid
- Wide Elf
ev: '6'
file_basename: Wode Elf Greenskeeper
file_dpath: Monsters/Elves Wode/Statblocks
free_strike: 3
intuition: 0
item_id: wode-elf-greenskeeper
item_index: '231'
item_name: Wode Elf Greenskeeper
level: 1
might: 0
presence: 1
reason: 0
roles:
- Platoon Defender
scc:
- mcdm.monsters.v1:monster:wode-elf-greenskeeper
scdc:
- 1.1.1:2:231
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '40'
type: monster
---

```ds-statblock
name: Wode Elf Greenskeeper
level: 1
roles:
  - Platoon Defender
ancestry:
  - Fey
  - Humanoid
  - Wide Elf
ev: "6"
stamina: "40"
speed: 7
size: 1M
stability: 0
free_strike: 3
might: 0
agility: 2
reason: 0
intuition: 0
presence: 1
traits:
  - name: Masking Glamor
    effects:
      - effect: Abilities targeting the greenskeeper that would take a bane from cover
          or concealment have a double bane instead.
abilities:
  - name: Growing Longsword
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 5 damage
        t2: 7 damage
        t3: 9 damage
      - effect: The target is taunted until the end of their next turn, and the
          greenskeeper shifts up to 3 squares
        name: Effect
      - effect: The distance increases to Melee 5.
        cost: 2 Malice
  - name: Overgrowth
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
      - Ranged
    type: Maneuver
    distance: 3 cube within 10
    target: Special
    effects:
      - effect: The area is overgrown with heavy brush and brambles until the end of the
          encounter, providing cover and concealment for the greenskeeper and
          their allies. The area is difficult terrain for enemies and any enemy
          who starts their turn in the area takes 3 damage.
        name: Effect
```