---
agility: 1
ancestry:
- Undead
ev: '3'
file_basename: Specter
file_dpath: Monsters/Undead/Statblocks
free_strike: 1
intuition: 0
item_id: specter
item_index: '66'
item_name: Specter
level: 1
might: -5
presence: 2
reason: 0
roles:
- Horde Hexer
scc:
- mcdm.monsters.v1:monster:specter
scdc:
- 1.1.1:2:66
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '10'
type: monster
---

```ds-statblock
name: Specter
level: 1
roles:
  - Horde Hexer
ancestry:
  - Undead
ev: "3"
stamina: "10"
immunities:
  - Corruption 1
  - poison 1
speed: 5
movement: Fly, hover
size: 1M
stability: 1
free_strike: 1
might: -5
agility: 1
reason: 0
intuition: 0
presence: 2
traits:
  - name: Corruptive Phasing
    effects:
      - effect: The specter can move through creatures and objects at their usual speed,
          but can't end their turn inside a creature or object. The first time
          in a round that the specter moves through a creature, that creature
          takes 2 corruption damage. The specter doesn't take damage from being
          force moved into objects.
abilities:
  - name: Decaying Touch
    cost: Signature Ability
    keywords:
      - Magic
      - Melee
      - Strike
    type: Main action
    distance: Melee 1
    target: One creature
    effects:
      - roll: Power Roll + 2
        t1: 3 corruption damage; P < 0 weakened (save ends)
        t2: 4 corruption damage; P < 1 weakened (save ends)
        t3: 5 corruption damage; P < 2 weakened (save ends)
      - effect: The potency increases by 1. Any living creature who dies from this
          damage rises at the start of the next round in the target's space as a
          specter under the Director's control.
        cost: 2 Malice
  - name: Hidden Movement
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The specter turns invisible, moves up to their speed, and is visible
          again.
        name: Effect
```