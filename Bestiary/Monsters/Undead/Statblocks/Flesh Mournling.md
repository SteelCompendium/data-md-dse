---
agility: 1
ancestry:
- Undead
ev: '6'
file_basename: Flesh Mournling
file_dpath: Monsters/Undead/Statblocks
free_strike: 2
intuition: 2
item_id: flesh-mournling
item_index: '83'
item_name: Flesh Mournling
level: 4
might: 3
presence: -1
reason: 0
roles:
- Horde Defender
scc:
- mcdm.monsters.v1:monster:flesh-mournling
scdc:
- 1.1.1:2:83
size: '2'
source: mcdm.monsters.v1
speed: 6
stability: 2
stamina: '35'
type: monster
---

```ds-statblock
name: Flesh Mournling
level: 4
roles:
  - Horde Defender
ancestry:
  - Undead
ev: "6"
stamina: "35"
immunities:
  - Corruption 4
  - poison 4
speed: 6
size: "2"
stability: 2
free_strike: 2
might: 3
agility: 1
reason: 0
intuition: 2
presence: -1
traits:
  - name: Arise
    effects:
      - effect: The first time the mournling is reduced to 0 Stamina by damage that
          isn't fire damage or holy damage and their body isn't destroyed, they
          instead have 10 Stamina and fall prone.
  - name: Immutable Form
    effects:
      - effect: The mournling's shape can't be changed by any external effect.
abilities:
  - name: Multiarm Strike
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        t1: 5 damage
        t2: 7 damage
        t3: 9 damage
      - effect: The target can't shift until the end of their next turn
        name: Effect
      - effect: This ability targets one additional target.
        cost: 1 Malice
  - name: Horrid Wail
    keywords:
      - Area
      - Magic
    type: Main action
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        t1: 2 psychic damage
        t2: 3 psychic damage; I < 2 frightened (save ends)
        t3: 4 psychic damage; I < 3 frightened (save ends)
      - effect: A target who is still frightened this way at the end of the encounter
          can't take a respite activity during their next respite.
        name: Effect
```