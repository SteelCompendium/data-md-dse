---
agility: 1
ancestry:
- Undead
- Soulless
ev: '12'
file_basename: Lithgekh
file_dpath: Monsters/Undead/Statblocks
free_strike: 5
intuition: 3
item_id: lithgekh
item_index: '63'
item_name: Lithgekh
level: 10
might: 0
presence: -1
reason: 5
roles:
- Horde Hexer
scc:
- mcdm.monsters.v1:monster:lithgekh
scdc:
- 1.1.1:2:63
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 1
stamina: '55'
type: monster
---

```ds-statblock
name: Lithgekh
level: 10
roles:
  - Horde Hexer
ancestry:
  - Undead
  - Soulless
ev: "12"
stamina: "55"
immunities:
  - Corruption 10
  - poison 10
speed: 6
movement: Fly, hover
size: 1M
stability: 1
free_strike: 5
might: 0
agility: 1
reason: 5
intuition: 3
presence: -1
traits:
  - name: Devour Magic
    effects:
      - effect: Each ally within 10 squares of the lithgekh gains an edge on magic
          abilities.
abilities:
  - name: Heartstopper
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 15
    target: One creature or object
    effects:
      - roll: Power Roll + 5
        t1: 9 corruption damage; I < 3 frightened (save ends)
        t2: 12 corruption damage; I < 4 frightened (save ends)
        t3: 14 corruption damage; I < 5 frightened (save ends)
      - effect: A creature frightened this way takes a bane on any ability that targets
          undead.
  - name: Mystic Battery
    cost: 1 Malice
    keywords:
      - Magic
      - Ranged
    type: Free triggered action
    distance: Ranged 20
    target: The triggering creature
    trigger: A creature within distance uses a magic ability.
    effects:
      - effect: Any damage dealt by or Stamina regained from the ability is halved. The
          lithgekh regains Stamina equal to the remaining damage dealt or
          Stamina gained.
```