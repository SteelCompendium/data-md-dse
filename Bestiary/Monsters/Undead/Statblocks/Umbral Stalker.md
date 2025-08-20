---
agility: 2
ancestry:
- Undead
ev: '3'
file_basename: Umbral Stalker
file_dpath: Monsters/Undead/Statblocks
free_strike: 2
intuition: 0
item_id: umbral-stalker
item_index: '58'
item_name: Umbral Stalker
level: 1
might: 0
presence: 1
reason: 0
roles:
- Horde Ambusher
scc:
- mcdm.monsters.v1:monster:umbral-stalker
scdc:
- 1.1.1:2:58
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 1
stamina: '15'
type: monster
---

```ds-statblock
name: Umbral Stalker
level: 1
roles:
  - Horde Ambusher
ancestry:
  - Undead
ev: "3"
stamina: "15"
immunities:
  - Corruption 1
  - poison 1
speed: 7
movement: Climb
size: 1M
stability: 1
free_strike: 2
might: 0
agility: 2
reason: 0
intuition: 0
presence: 1
traits:
  - name: Corruptive Phasing
    effects:
      - effect: The umbral stalker can move through creatures and objects at their usual
          speed, but can't end their turn inside a creature or object. The first
          time in a round that the umbral stalker moves through a creature, that
          creature takes 2 corruption damage. The umbral stalker doesn't take
          damage from being force moved into objects.
abilities:
  - name: Chilling Grasp
    cost: Signature Ability
    keywords:
      - Magic
      - Melee
      - Strike
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 4 cold damage
        t2: 6 cold damage; the stalker can shift 1 square
        t3: 7 cold damage; the stalker shifts up to 2 squares
  - name: Freezing Dark
    cost: 3 Malice
    keywords:
      - Area
      - Magic
    type: Main action
    distance: 3 cube within 1
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        t1: 2 cold damage
        t2: 3 cold damage
        t3: 4 cold damage
      - effect: Until the end of the stalker's next turn, the area provides concealment,
          and blocks line of effect for enemies
  - name: Shadow Jump
    cost: 1 Malice
    keywords:
      - "-"
    type: Free maneuver
    distance: Self
    target: Self
    effects:
      - effect: The umbral stalker teleports to an unoccupied space in an area of
          concealment within 10 squares.
```