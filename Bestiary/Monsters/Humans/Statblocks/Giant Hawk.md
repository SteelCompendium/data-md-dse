---
agility: 2
ancestry:
- Animal
- Human
ev: '6'
file_basename: Giant Hawk
file_dpath: Monsters/Humans/Statblocks
free_strike: 3
intuition: 1
item_id: giant-hawk
item_index: '168'
item_name: Giant Hawk
level: 1
might: 2
presence: -2
reason: -3
roles:
- Platoon Mount
scc:
- mcdm.monsters.v1:monster:giant-hawk
scdc:
- 1.1.1:2:168
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '30'
type: monster
---

~~~ds-statblock
name: Giant Hawk
level: 1
roles:
  - Platoon Mount
ancestry:
  - Animal
  - Human
ev: "6"
stamina: "30"
speed: 5
movement: Fly
size: "2"
stability: 0
free_strike: 3
might: 2
agility: 2
reason: -3
intuition: 1
presence: -2
traits:
  - name: Mounted Platform
    effects:
      - effect: Once per turn when the hawk moves, any creature riding the hawk can make
          a free strike during or after the movement.
abilities:
  - name: Talons
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 5 damage
        t2: 7 damage
        t3: 9 damage; grabbed
      - effect: If this ability gains an edge or has a double edge, it deals an extra 2
          damage.
        cost: 2 Malice
  - name: Dive
    icon: 👤
    cost: 1 Malice
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The hawk moves up to their speed.
        name: Effect
~~~