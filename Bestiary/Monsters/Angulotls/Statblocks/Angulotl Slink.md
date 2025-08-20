---
agility: 2
ancestry:
- Angulotl
- Humanoid
ev: '3'
file_basename: Angulotl Slink
file_dpath: Monsters/Angulotls/Statblocks
free_strike: 2
intuition: 0
item_id: angulotl-slink
item_index: '238'
item_name: Angulotl Slink
level: 1
might: 1
presence: 0
reason: 0
roles:
- Horde Ambusher
scc:
- mcdm.monsters.v1:monster:angulotl-slink
scdc:
- 1.1.1:2:238
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '15'
type: monster
---

```ds-statblock
name: Angulotl Slink
level: 1
roles:
  - Horde Ambusher
ancestry:
  - Angulotl
  - Humanoid
ev: "3"
stamina: "15"
immunities:
  - Poison 2
speed: 5
movement: Climb, swim
size: 1S
stability: 0
free_strike: 2
might: 1
agility: 2
reason: 0
intuition: 0
presence: 0
traits:
  - name: Adhesive
    effects:
      - effect: The slink excretes a sticky residue into their square at the end of each
          of their turns. Any non-angulotl who enters or leaves the square is
          stuck, and must use a maneuver to break free or be restrained until
          the end of their turn. Objects are likewise affected, and a creature
          must use a maneuver to remove an object from the square.
  - name: Toxiferous
    effects:
      - effect: Whenever an adjacent enemy grabs the slink or uses a melee ability
          against them, that enemy takes 2 poison damage.
abilities:
  - name: Tonguelash
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 6
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 4 damage; pull 2
        t2: 6 damage; pull 4
        t3: 7 damage; pull 6
      - effect: The target is wet (save ends). Any ally targeted by this ability ignores
          the damage, is wet until the end of the encounter, and is pulled up to
          6 squares, ignoring stability.
  - name: Hop To It
    cost: 2 Malice
    keywords:
      - "-"
    type: Free maneuver
    distance: Self
    target: Self
    effects:
      - effect: The slink jumps up to 3 squares. If they have cover or concealment when
          they land, they can attempt to hide.
```