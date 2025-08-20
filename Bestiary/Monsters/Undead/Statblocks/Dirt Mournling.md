---
agility: 1
ancestry:
- Undead
ev: '9'
file_basename: Dirt Mournling
file_dpath: Monsters/Undead/Statblocks
free_strike: 3
intuition: 1
item_id: dirt-mournling
item_index: '74'
item_name: Dirt Mournling
level: 7
might: 4
presence: -3
reason: -2
roles:
- Horde Controller
scc:
- mcdm.monsters.v1:monster:dirt-mournling
scdc:
- 1.1.1:2:74
size: '3'
source: mcdm.monsters.v1
speed: 6
stability: 3
stamina: '64'
type: monster
---

```ds-statblock
name: Dirt Mournling
level: 7
roles:
  - Horde Controller
ancestry:
  - Undead
ev: "9"
stamina: "64"
immunities:
  - Corruption 7
  - poison 7
speed: 6
movement: Burrow, climb
size: "3"
stability: 3
free_strike: 3
might: 4
agility: 1
reason: -2
intuition: 1
presence: -3
traits:
  - name: Arise
    effects:
      - effect: The first time the mournling is reduced to 0 Stamina by damage that
          isn't fire damage or holy damage and their body isn't destroyed, they
          instead have 15 Stamina and fall prone.
  - name: Immutable Form
    effects:
      - effect: The mournling's shape can't be changed by any external effect
  - name: Rupture
    effects:
      - effect: Whenever the mournling uses the Dig maneuver to breach the surface, they
          make a free strike against each adjacent enemy.
abilities:
  - name: Mudslide
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        t1: 7 damage; M < 3 grabbed
        t2: 10 damage; M < 4 grabbed
        t3: 11 damage; grabbed
      - effect: A 3-cube area of ground centered on the target is difficult terrain for
          enemies.
  - name: Mourning Cry
    cost: 3 Malice
    keywords:
      - Area
      - Magic
    type: Main action
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        t1: 3 corruption damage; I < 2 frightened (save ends)
        t2: 6 corruption damage; I < 3 frightened (save ends)
        t3: 7 corruption damage; I < 4 frightened (save ends)
      - effect: A target frightened this way is frightened of all undead. This effect
          ends early if the mournling is destroyed
```