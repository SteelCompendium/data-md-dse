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

```ds-statblock
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
traits:
  - name: Masking Glamor
    effects:
      - effect: Abilities targeting the green seer that would take a bane from cover or
          concealment have a double bane instead.
abilities:
  - name: The Forest's Embrace
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 5 damage
        t2: 7 damage; I < 1 restrained (save ends)
        t3: 9 damage; I < 2 restrained (save ends)
      - effect: While restrained this way, a target can't search for hidden creatures.
        name: Effect
  - name: The Natural Cycle
    icon: 🏹
    cost: 3 Malice
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Maneuver
    distance: Ranged 10
    target: Two creatures
    effects:
      - roll: Power Roll + 2
        t1: 2 damage
        t2: 4 damage; P < 1 weakened (save ends)
        t3: 6 damage; P < 1 bleeding (save ends); the target has a double bane on
          strikes (save ends)
      - effect: While bleeding or weakened this way, a target is covered in lichen.
        name: Effect
  - name: Foreseen Punishment
    icon: ❗️
    keywords:
      - Ranged
    type: Free triggered action
    distance: Ranged 5
    target: The triggering creature
    trigger: A creature uses a triggered action targeting the green seer or an ally
      within distance.
    effects:
      - effect: The green seer makes a free strike against the target after the target's
          triggered action is resolved.
        name: Effect
```