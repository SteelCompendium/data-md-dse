---
agility: 2
ancestry:
- Draconian
- Dragon
- Humanoid
ev: '32'
file_basename: Aeolyxria the Uncanny
file_dpath: Monsters/Draconians/Statblocks
free_strike: 7
intuition: 3
item_id: aeolyxria-the-uncanny
item_index: '104'
item_name: Aeolyxria the Uncanny
level: 6
might: -1
presence: 1
reason: 2
roles:
- Elite Controller
scc:
- mcdm.monsters.v1:monster:aeolyxria-the-uncanny
scdc:
- 1.1.1:2:104
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '140'
type: monster
---

```ds-statblock
name: Aeolyxria the Uncanny
level: 6
roles:
  - Elite Controller
ancestry:
  - Draconian
  - Dragon
  - Humanoid
ev: "32"
stamina: "140"
immunities:
  - Poison 6
speed: 5
movement: Fly
size: 1M
stability: 2
free_strike: 7
might: -1
agility: 2
reason: 2
intuition: 3
presence: 1
traits:
  - name: That's Our Opening!
    effects:
      - effect: The Director gains 1 Malice whenever Aeolyxria imposes a condition on an
          enemy.
abilities:
  - name: Spittlesplash
    cost: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 10
    target: Two enemies
    effects:
      - roll: Power Roll + 3
        t1: 10 poison damage; M < 1 slowed (save ends)
        t2: 15 poison damage; M < 2 slowed (save ends)
        t3: 18 poison damage; M < 3 slowed (save ends)
  - name: Experimental Treasure
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 10
    target: Two creature or objects
    effects:
      - roll: Power Roll + 3
        t1: The targets regains 10 Stamina.
        t2: 12 corruption damage; A < 2 weakened (save ends)
        t3: 12 lightning damage; A < 2 bleeding (save ends)
      - effect: The first time in an encounter that Aeolyxria makes a power roll for
          this ability, she can subsequently use the outcome of that roll
          instead of rolling whenever she uses this ability until the end of the
          encounter.
        name: Effect
      - effect: The ability targets one additional target for each 2 Malice spent.
        cost: 2+ Malice
  - name: Elevate
    cost: 2 Malice
    keywords:
      - Area
      - Ranged
    type: Maneuver
    distance: 1 cube within 5
    target: Special
    effects:
      - effect: The ground in the area rises 5 squares, creating a pillar of dirt. Any
          creature in the area moves with the ground to its new elevation.
        name: Effect
      - effect: Aeolyxria creates an additional pillar for each Malice spent.
        cost: 1+ Malice
  - name: Blood For Blood
    keywords:
      - Ranged
      - Weapon
    type: Triggered action
    distance: Ranged 5
    target: One creature
    trigger: An ally is made bleeding by the target.
    effects:
      - roll: Power Roll + 3
        t1: 7 poison damage; A < 2 bleeding (save ends)
        t2: 12 poison damage; A < 3 bleeding (save ends)
        t3: 15 poison damage; bleeding (save ends)
```