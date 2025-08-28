---
agility: 1
ancestry:
- Goblin
- Humanoid
ev: '3'
file_basename: Goblin Stinker
file_dpath: Monsters/Goblins/Statblocks
free_strike: 1
intuition: 0
item_id: goblin-stinker
item_index: '312'
item_name: Goblin Stinker
level: 1
might: -2
presence: 2
reason: 0
roles:
- Horde Controller
scc:
- mcdm.monsters.v1:monster:goblin-stinker
scdc:
- 1.1.1:2:312
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '10'
type: monster
---

~~~ds-statblock
name: Goblin Stinker
level: 1
roles:
  - Horde Controller
ancestry:
  - Goblin
  - Humanoid
ev: "3"
stamina: "10"
speed: 5
movement: Climb
size: 1S
stability: 0
free_strike: 1
might: -2
agility: 1
reason: 0
intuition: 0
presence: 2
traits:
  - name: Crafty
    effects:
      - effect: The stinker doesn't provoke opportunity attacks by moving
abilities:
  - name: Toxic Winds
    icon: 🔳
    cost: Signature Ability
    keywords:
      - Area
      - Magic
      - Ranged
    type: Main action
    distance: 3 cube within 15
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        t1: 1 poison damage; slide 1
        t2: 2 poison damage; slide 2
        t3: 3 poison damage; slide 3
      - effect: For each Malice spent, one target can be force moved 1 additional
          square.
        cost: 1+ Malice
  - name: Swamp Gas
    icon: 🔳
    keywords:
      - Area
      - Magic
      - Ranged
    type: Maneuver
    distance: 3 cube within 10
    target: Special
    effects:
      - effect: The area is filled with a green haze that lasts until the start of the
          stinker's next turn or until the stinker is reduced to 0 Stamina, and
          which can't be dispersed by wind. The area is difficult terrain for
          non-goblins, and each non-goblin who moves in the area takes 2 poison
          damage for each square moved.
        name: Effect
~~~