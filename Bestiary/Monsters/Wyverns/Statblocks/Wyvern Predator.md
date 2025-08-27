---
agility: 2
ancestry:
- Beast
- Wyvern
ev: '24'
file_basename: Wyvern Predator
file_dpath: Monsters/Wyverns/Statblocks
free_strike: 6
intuition: 1
item_id: wyvern-predator
item_index: '122'
item_name: Wyvern Predator
level: 4
might: 3
presence: 0
reason: -1
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:wyvern-predator
scdc:
- 1.1.1:2:122
size: '3'
source: mcdm.monsters.v1
speed: 7
stability: 3
stamina: '140'
type: monster
---

```ds-statblock
name: Wyvern Predator
level: 4
roles:
  - Elite Brute
ancestry:
  - Beast
  - Wyvern
ev: "24"
stamina: "140"
immunities:
  - Acid 5
speed: 7
movement: Fly
size: "3"
stability: 3
free_strike: 6
might: 3
agility: 2
reason: -1
intuition: 1
presence: 0
traits:
  - name: Stubborn Rage
    effects:
      - effect: While winded or within 10 squares of another wyvern, the predator can't
          be made dazed or frightened.
  - name: Tenacious Hunter
    effects:
      - effect: Any creature affected by a condition imposed by a wyvern can't be hidden
          from the predator.
abilities:
  - name: Sedating Stinger
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Magic
      - Strike
      - Weapon
    type: Main action
    distance: Melee 3
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        t1: 9 damage
        t2: 14 damage; M < 2 slowed (save ends)
        t3: 17 damage; M < 3 slowed (save ends)
      - effect: If a target slowed this way is already slowed, they are instead
          restrained (save ends).
        name: Effect
  - name: Tail Sweep
    icon: 🔳
    keywords:
      - Area
      - Weapon
    type: Main action
    distance: 6 x 3 line within 1
    target: Each enemy and object in the area
    effects:
      - roll: Power Roll + 3
        t1: 6 damage; A < 1 3 acid damage
        t2: 11 damage; A < 2 3 acid damage
        t3: 14 damage; A < 3 3 acid damage
      - effect: The predator uses this ability a second time, either recreating the same
          line or creating a new line.
        cost: 5 Malice
  - name: Grasping Jaws
    icon: 🗡
    cost: 2 Malice
    keywords:
      - Magic
      - Strike
      - Weapon
    type: Maneuver
    distance: Melee 2
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        t1: 9 damage; A < 1 grabbed
        t2: 14 damage; A < 2 grabbed
        t3: 17 damage; A < 3 grabbed and the target takes a bane on the Escape Grab
          maneuver
  - name: Deterring Sting
    icon: ❗️
    cost: 1 Malice
    keywords:
      - Melee
    type: Triggered action
    distance: Melee 3
    target: The triggering creature
    trigger: A creature within distance deals damage to the predator with a melee
      ability.
    effects:
      - effect: The predator uses Sedating Stinger against the target, then shifts up to
          3 squares
        name: Effect
```