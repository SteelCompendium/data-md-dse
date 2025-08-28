---
agility: 2
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '3'
file_basename: War Dog Teletalite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 2
intuition: 0
item_id: war-dog-teletalite
item_index: '376'
item_name: War Dog Teletalite
level: 1
might: 0
presence: 0
reason: 0
roles:
- Horde Ambusher
scc:
- mcdm.monsters.v1:monster:war-dog-teletalite
scdc:
- 1.1.1:2:376
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '15'
type: monster
---

~~~ds-statblock
name: War Dog Teletalite
level: 1
roles:
  - Horde Ambusher
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "3"
stamina: "15"
speed: 5
movement: Teleport
size: 1M
stability: 0
free_strike: 2
might: 0
agility: 2
reason: 0
intuition: 0
presence: 0
traits:
  - name: Loyalty Collar
    effects:
      - effect: When the teletalite is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 1d6 damage to each adjacent enemy and object.
abilities:
  - name: Corrupted Ash Daggers
    icon: ⚔️
    cost: Signature Ability
    keywords:
      - Melee
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1 or ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 4 damage; slide 1
        t2: 6 damage; slide 2
        t3: 7 damage; slide 3
      - effect: The teletalite gains an edge on this ability if any ally is adjacent to
          the target.
        name: Effect
      - effect: The teletalite teleports the target 3 squares before sliding them.
        cost: 1 Malice
  - name: Posthumous Promotion
    icon: 🏹
    keywords:
      - Magic
      - Ranged
    type: Maneuver
    distance: Ranged 10
    target: One war dog
    effects:
      - effect: If the target has a loyalty collar, they are reduced to 0 Stamina.
        name: Effect
  - name: Corrupted Ash Teleport
    icon: 👤
    cost: 1 Malice
    keywords:
      - Magic
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The teletalite can teleport up to 5 squares and gains an edge on strikes
          until the end of their turn.
        name: Effect
~~~