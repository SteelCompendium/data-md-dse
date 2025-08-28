---
agility: 2
ancestry:
- Animal
ev: '12'
file_basename: Big Animal A
file_dpath: Monsters/Animals/Statblocks
free_strike: 4
intuition: 1
item_id: big-animal-a
item_index: '249'
item_name: Big Animal A
level: 1
might: 1
presence: -2
reason: -2
roles:
- Elite Mount
scc:
- mcdm.monsters.v1:monster:big-animal-a
scdc:
- 1.1.1:2:249
size: '2'
source: mcdm.monsters.v1
speed: 6
stability: 1
stamina: '60'
type: monster
---

```ds-statblock
name: Big Animal A
level: 1
roles:
  - Elite Mount
ancestry:
  - Animal
ev: "12"
stamina: "60"
speed: 6
size: "2"
stability: 1
free_strike: 4
might: 1
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
        t2: 9 damage; A < 1 3 damage
        t3: 12 damage; A < 2 3 damage
  - name: Toss
    icon: 🗡
    keywords:
      - Melee
    type: Maneuver
    distance: Melee 1
    target: One creature or object
    effects:
      - effect: The target must be the animal's size or smaller.
        name: Special
      - effect: The target vertical slides up to 3 squares. If the target is an ally,
          they can make a free strike at the end of the forced movement, then
          fall without taking damage.
        name: Effect
  - name: ❗️**Juke**
    keywords:
      - "-"
    type: Triggered action
    distance: Self
    target: Self
    trigger: The animal is targeted by an area ability.
    effects:
      - effect: The animal shifts up to 2 squares before the ability resolves.
        name: Effect
```