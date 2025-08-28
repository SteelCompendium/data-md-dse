---
agility: 2
ancestry:
- Humanoid
- Lizardfolk
ev: '6'
file_basename: Lizardfolk Skyterror
file_dpath: Monsters/Lizardfolks/Statblocks
free_strike: 3
intuition: 0
item_id: lizardfolk-skyterror
item_index: '48'
item_name: Lizardfolk Skyterror
level: 1
might: 1
presence: 1
reason: 0
roles:
- Platoon Harrier
scc:
- mcdm.monsters.v1:monster:lizardfolk-skyterror
scdc:
- 1.1.1:2:48
size: 1S
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '30'
type: monster
---

~~~ds-statblock
name: Lizardfolk Skyterror
level: 1
roles:
  - Platoon Harrier
ancestry:
  - Humanoid
  - Lizardfolk
ev: "6"
stamina: "30"
speed: 7
movement: Swim
size: 1S
stability: 0
free_strike: 3
might: 1
agility: 2
reason: 0
intuition: 0
presence: 1
traits:
  - name: Glider
    effects:
      - effect: Whenever the skyterror moves 2 or more squares along the ground or falls
          2 or more squares, they can fly until the end of their next turn.
  - name: Reptilian Escape
    effects:
      - effect: While the skyterror has a tail, whenever they are grabbed, prone,
          slowed, or weakened, they can lose their tail to immediately end that
          condition, then shift up to 2 squares.
abilities:
  - name: Glaive Rush
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
        t3: 9 damage; prone
      - effect: If the skyterror is flying, they shift up to 4 squares.
        name: Effect
  - name: Poison Blow Dart
    icon: 🏹
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 5
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 3 damage; M < 0 weakened (save ends)
        t2: 5 damage; M < 1 weakened (save ends)
        t3: 7 damage; M < 2 weakened (save ends)
      - effect: Any creature who ends their turn adjacent to a target weakened this way
          is weakened until the end of their next turn.
        name: Effect
~~~