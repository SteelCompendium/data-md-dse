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
item_index: '236'
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
- 1.1.1:2:236
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '15'
type: monster
---

~~~ds-statblock
type: statblock
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
features:
  - type: feature
    feature_type: ability
    name: Tonguelash
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 6
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 4 damage; pull 2
        tier2: 6 damage; pull 4
        tier3: 7 damage; pull 6
      - name: Effect
        effect: The target is wet (save ends). Any ally targeted by this ability ignores
          the damage, is wet until the end of the encounter, and is pulled up to
          6 squares, ignoring stability.
  - type: feature
    feature_type: ability
    name: Hop To It
    icon: 👤
    cost: 2 Malice
    keywords:
      - "-"
    usage: Free maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The slink jumps up to 3 squares. If they have cover or concealment when
          they land, they can attempt to hide.
  - type: feature
    feature_type: trait
    name: Adhesive
    icon: ⭐️
    effects:
      - effect: The slink excretes a sticky residue into their square at the end of each
          of their turns. Any non-angulotl who enters or leaves the square is
          stuck, and must use a maneuver to break free or be restrained until
          the end of their turn. Objects are likewise affected, and a creature
          must use a maneuver to remove an object from the square.
  - type: feature
    feature_type: trait
    name: Toxiferous
    icon: ⭐️
    effects:
      - effect: Whenever an adjacent enemy grabs the slink or uses a melee ability
          against them, that enemy takes 2 poison damage.
~~~