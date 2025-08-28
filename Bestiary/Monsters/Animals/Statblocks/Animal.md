---
agility: 2
ancestry:
- Animal
ev: '12'
file_basename: Animal
file_dpath: Monsters/Animals/Statblocks
free_strike: 4
intuition: 1
item_id: animal
item_index: '251'
item_name: Animal
level: 1
might: 0
presence: -2
reason: -2
roles:
- Elite Harrier
scc:
- mcdm.monsters.v1:monster:animal
scdc:
- 1.1.1:2:251
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '60'
type: monster
---

~~~ds-statblock
name: Animal
level: 1
roles:
  - Elite Harrier
ancestry:
  - Animal
ev: "12"
stamina: "60"
speed: 6
size: 1M
stability: 0
free_strike: 4
might: 0
agility: 2
reason: -2
intuition: 1
presence: -2
traits:
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
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        t1: 6 damage
        t2: 9 damage
        t3: 12 damage
      - effect: The animal shifts up to 2 squares between strikes.
        name: Effect
  - name: Rush
    icon: 👤
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The animal moves up to their speed.
        name: Effect
~~~