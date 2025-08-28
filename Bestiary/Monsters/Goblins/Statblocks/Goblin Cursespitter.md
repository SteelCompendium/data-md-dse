---
agility: 1
ancestry:
- Goblin
- Humanoid
ev: '3'
file_basename: Goblin Cursespitter
file_dpath: Monsters/Goblins/Statblocks
free_strike: 1
intuition: 2
item_id: goblin-cursespitter
item_index: '305'
item_name: Goblin Cursespitter
level: 1
might: -2
presence: 0
reason: 0
roles:
- Horde Hexer
scc:
- mcdm.monsters.v1:monster:goblin-cursespitter
scdc:
- 1.1.1:2:305
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '10'
type: monster
---

~~~ds-statblock
name: Goblin Cursespitter
level: 1
roles:
  - Horde Hexer
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
intuition: 2
presence: 0
traits:
  - name: Crafty
    effects:
      - effect: The cursespitter doesn't provoke opportunity attacks by moving.
abilities:
  - name: Eye of Surlach
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 15
    target: One creature
    effects:
      - roll: Power Roll + 2
        t1: 3 corruption damage; I < 0 weakened (save ends)
        t2: 5 corruption damage; I < 2 weakened (save ends)
  - name: Dizzying Hex
    icon: 🏹
    cost: 1 Malice
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Maneuver
    distance: Ranged 10
    target: One creature
    effects:
      - roll: Power Roll + 2
        t1: I < 0 prone
        t2: I < 1 prone and can't stand (EoT)
        t3: Prone; I < 2 can't stand (save ends)
~~~