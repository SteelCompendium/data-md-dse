---
agility: 2
ancestry:
- Animal
ev: '12'
file_basename: Predator A
file_dpath: Monsters/Animals/Statblocks
free_strike: 5
intuition: 1
item_id: predator-a
item_index: '252'
item_name: Predator A
level: 1
might: 1
presence: 1
reason: -2
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:predator-a
scdc:
- 1.1.1:2:252
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '80'
type: monster
---

```ds-statblock
name: Predator A
level: 1
roles:
  - Elite Brute
ancestry:
  - Animal
ev: "12"
stamina: "80"
speed: 5
size: "2"
stability: 0
free_strike: 5
might: 1
agility: 2
reason: -2
intuition: 1
presence: 1
traits:
  - name: Nature's Spirit
    effects:
      - effect: While outdoors or in a natural environment, the predator can negate a
          bane on their abilities or turn a double bane into a bane.
abilities:
  - name: Natural Weapon
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
        t1: 7 damage
        t2: 10 damage; M < 1 prone
        t3: 13 damage; M < 1 prone
  - name: Ready to Strike
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The predator assesses their environment or lets loose a threatening roar
          and gains an edge on their next strike.
  - name: Quick Strike
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Triggered action
    distance: Melee 1
    target: The triggering creature or object
    trigger: A creature or object comes within distance.
    effects:
      - effect: The predator makes a free strike against the target. If the predator was
          hidden from the target, the strike deals an extra 3 damage.
```