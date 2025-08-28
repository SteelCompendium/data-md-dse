---
agility: 3
ancestry:
- Giant
- Stone Giant
ev: '40'
file_basename: Marble Stone Giant
file_dpath: Monsters/Giants/Statblocks
free_strike: 8
intuition: 3
item_id: marble-stone-giant
item_index: '201'
item_name: Marble Stone Giant
level: 8
might: 4
presence: 0
reason: 0
roles:
- Elite Hexer
scc:
- mcdm.monsters.v1:monster:marble-stone-giant
scdc:
- 1.1.1:2:201
size: '4'
source: mcdm.monsters.v1
speed: 6
stability: 10
stamina: '207'
type: monster
---

```ds-statblock
name: Marble Stone Giant
level: 8
roles:
  - Elite Hexer
ancestry:
  - Giant
  - Stone Giant
ev: "40"
stamina: "207"
speed: 6
movement: Burrow
size: "4"
stability: 10
free_strike: 8
might: 4
agility: 3
reason: 0
intuition: 3
presence: 0
traits:
  - name: Stonebreaker Flesh
    effects:
      - effect: Whenever an enemy obtains a tier 1 outcome on a melee ability used
          against the marble stone giant, they take a bane on that ability until
          the end of the encounter.
  - name: Stone Steps
    effects:
      - effect: The marble stone giant ignores difficult terrain.
  - name: Stone Swim
    effects:
      - effect: The marble stone giant can burrow through stone, but can't drag other
          creatures underground when they do so.
abilities:
  - name: Marble From a Great Sling
    icon: 🔳
    cost: Signature Ability
    keywords:
      - Area
      - Ranged
      - Weapon
    type: Main action
    distance: 3 cube within 15
    target: Each enemy and object in the area
    effects:
      - roll: Power Roll + 4
        t1: 6 damage; I < 2 dazed (save ends)
        t2: 10 damage; I < 3 dazed (save ends)
        t3: 14 damage; I < 4 dazed (save ends)
      - effect: If the target has any effect on them that can be ended by a saving throw
          or that ends at the end of their turn, they are also knocked prone.
        name: Effect
  - name: Far Flung
    icon: 🗡
    cost: 3 Malice
    keywords:
      - Melee
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        t1: Vertical push 7
        t2: Vertical push 10
        t3: Vertical push 12
      - effect: Against a target who is prone or grabbed, this ability has a double
          edge.
        name: Effect
  - name: Polish Stone Shape
    icon: 🔳
    keywords:
      - Area
    type: Maneuver
    distance: 10 x 2 line within 1
    target: Special
    effects:
      - effect: The ground in the area becomes slick and glossy. Any non-giant who
          starts or ends their turn in the area is knocked prone and slides 2
          squares.
        name: Effect
  - name: Break Armor
    icon: ❗️
    cost: 1 Malice
    keywords:
      - "-"
    type: Triggered action
    distance: Self
    target: Self
    trigger: The marble stone giant takes damage.
    effects:
      - effect: The marble stone giant halves the damage, and has damage weakness 3 and
          a +3 bonus to speed until the end of the encounter. The damage
          weakness increases by 3 each time the marble stone giant uses this
          ability in the same encounter.
        name: Effect
```