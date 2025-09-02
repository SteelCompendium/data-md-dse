---
agility: 1
ancestry:
- Animal
ev: '16'
file_basename: Predator B
file_dpath: Monsters/Animals/Statblocks
free_strike: 5
intuition: 1
item_id: predator-b
item_index: '248'
item_name: Predator B
level: 3
might: 2
presence: 0
reason: -1
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:predator-b
scdc:
- 1.1.1:2:248
size: '3'
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '100'
type: monster
---

~~~ds-statblock
name: Predator B
level: 3
roles:
  - Elite Brute
ancestry:
  - Animal
ev: "16"
stamina: "100"
speed: 5
size: "3"
stability: 2
free_strike: 5
might: 2
agility: 1
reason: -1
intuition: 1
presence: 0
traits:
  - name: Trample
    effects:
      - effect: The predator can move through enemies' and objects' spaces at their
          usual speed. Any mundane size 2 or smaller object whose space they
          move through is destroyed. When the predator enters a creature's space
          for the first time on a turn, that creature takes 3 damage.
  - name: Nature's Spirit
    effects:
      - effect: While outdoors or in a natural environment, the predator can negate a
          bane on their abilities or turn a double bane into a bane.
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
        t2: 11 damage; push 1; M < 1 prone
        t3: 14 damage; push 2; M < 1 prone
  - name: Wild Swing
    icon: ❇️
    keywords:
      - Area
      - Weapon
    type: Main action
    distance: 1 burst
    target: Each enemy or object in the area
    effects:
      - roll: Power Roll + 2
        t1: 3 damage
        t2: 6 damage
        t3: 8 damage; A < 2 bleeding (save ends)
  - name: Swat
    icon: ❗️
    keywords:
      - Melee
    type: Triggered action
    distance: Melee 1
    target: The triggering creature or object
    trigger: A creature or object within distance deals damage to the predator.
    effects:
      - effect: The target is pushed up to 5 squares.
        name: Effect
~~~