---
agility: -2
ancestry:
- Undead
- Soulless
ev: '12'
file_basename: Bonecage
file_dpath: Monsters/Undead/Statblocks
free_strike: 4
intuition: 3
item_id: bonecage
item_index: '55'
item_name: Bonecage
level: 10
might: 5
presence: -1
reason: -2
roles:
- Horde Controller
scc:
- mcdm.monsters.v1:monster:bonecage
scdc:
- 1.1.1:2:55
size: '3'
source: mcdm.monsters.v1
speed: 6
stability: 5
stamina: '55'
type: monster
---

```ds-statblock
name: Bonecage
level: 10
roles:
  - Horde Controller
ancestry:
  - Undead
  - Soulless
ev: "12"
stamina: "55"
immunities:
  - Corruption 10
  - poison 10
speed: 6
movement: Climb
size: "3"
stability: 5
free_strike: 4
might: 5
agility: -2
reason: -2
intuition: 3
presence: -1
traits: []
abilities:
  - name: Ribcage Chomp
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 5
        t1: 9 damage; M < 4 grabbed
        t2: 12 damage; M < 5 grabbed
        t3: 14 damage; grabbed
      - effect: The bonecage can have up to four size 1 targets grabbed at once. Any
          creature grabbed by the bonecage takes a bane on the Escape Grab
          maneuver, and the bonecage has damage immunity 5 against that
          creature's abilities. When the bonecage is force moved, any creature
          or object they have grabbed moves with them.
        name: Effect
      - effect: While grabbed this way, a target can't teleport or be teleported.
        cost: 3 Malice
  - name: Labyrinth of Bone
    cost: 5 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    type: Main action
    distance: Four 10 x 1 lines within 3
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: The bonecage can put up to two 90-degree bends in each of the lines.
          Each target makes an Agility test.
        t1: 9 damage
        t2: 7 damage
        t3: 4 damage
      - effect: The area is difficult terrain for enemies. The effect ends at the end of
          the encounter or when the bonecage uses this ability again.
        name: Effect
```