---
agility: 1
ancestry:
- Animal
ev: '16'
file_basename: Big Animal B
file_dpath: Monsters/Animals/Statblocks
free_strike: 5
intuition: 1
item_id: big-animal-b
item_index: '253'
item_name: Big Animal B
level: 2
might: 2
presence: 0
reason: -1
roles:
- Elite Mount
scc:
- mcdm.monsters.v1:monster:big-animal-b
scdc:
- 1.1.1:2:253
size: '3'
source: mcdm.monsters.v1
speed: 6
stability: 3
stamina: '80'
type: monster
---

```ds-statblock
name: Big Animal B
level: 2
roles:
  - Elite Mount
ancestry:
  - Animal
ev: "16"
stamina: "80"
speed: 6
size: "3"
stability: 3
free_strike: 5
might: 2
agility: 1
reason: -1
intuition: 1
presence: 0
traits:
  - name: Beast of Burden
    effects:
      - effect: While riding the animal, two size 1 allies can occupy the same space.
  - name: Nature's Spirit
    effects:
      - effect: While outdoors or in a natural environment, the animal can negate a bane
          on their abilities or turn a double bane into a bane.
abilities:
  - name: Natural Weapon
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        t1: 7 damage
        t2: 10 damage; push 1
        t3: 13 damage; push 2
  - name: Trundle
    icon: 👤
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The animal moves up to their speed. They can make a free strike against
          each creature who makes an opportunity attack against them during this
          movement.
        name: Effect
  - name: Animal Rally
    icon: ❗️
    keywords:
      - "-"
    type: Triggered action
    distance: Ranged 20
    target: One ally
    trigger: The target is knocked prone.
    effects:
      - effect: The animal moves up to their speed. If they end their turn adjacent to
          the target, they can use the Stand Up maneuver to let the target
          stand, then get on to ride them.
        name: Effect
```