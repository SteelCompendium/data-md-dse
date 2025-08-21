---
agility: -1
ancestry:
- Undead
- Soulless
ev: '24'
file_basename: Giant Zombie
file_dpath: Monsters/Undead/Statblocks
free_strike: 6
intuition: 1
item_id: giant-zombie
item_index: '67'
item_name: Giant Zombie
level: 4
might: 3
presence: 2
reason: -2
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:giant-zombie
scdc:
- 1.1.1:2:67
size: '3'
source: mcdm.monsters.v1
speed: 6
stability: 2
stamina: '140'
type: monster
---

```ds-statblock
name: Giant Zombie
level: 4
roles:
  - Elite Brute
ancestry:
  - Undead
  - Soulless
ev: "24"
stamina: "140"
immunities:
  - Corruption 4
  - poison 4
speed: 6
size: "3"
stability: 2
free_strike: 6
might: 3
agility: -1
reason: -2
intuition: 1
presence: 2
traits:
  - name: Endless Knight
    effects:
      - effect: The first time the giant zombie is reduced to 0 Stamina by damage that
          isn't fire damage or holy damage and their body isn't destroyed, they
          instead have 50 Stamina and fall prone.
  - name: Negative Nerves
    effects:
      - effect: When the giant zombie is targeted by an ability that deals rolled
          damage, they halve the damage from a tier 1 outcome
abilities:
  - name: Rotten Smash
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 3
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        t1: 9 damage
        t2: 14 damage; A < 2 grabbed
        t3: 17 damage; A < 3 grabbed
  - name: Knocking Heads
    cost: 1 Malice
    keywords:
      - "-"
    type: Triggered action
    distance: Self
    target: Self; see below
    trigger: The giant zombie grabs two creatures or objects, or starts their turn
      with two creatures or objects grabbed.
    effects:
      - effect: The creatures or objects are smashed together using Rotten Smash, which
          has a double edge.
        name: Effect
```