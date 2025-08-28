---
agility: 2
ancestry:
- Goblin
- Humanoid
ev: '3'
file_basename: Goblin Warrior
file_dpath: Monsters/Goblins/Statblocks
free_strike: 1
intuition: 0
item_id: goblin-warrior
item_index: '304'
item_name: Goblin Warrior
level: 1
might: -2
presence: -1
reason: 0
roles:
- Horde Harrier
scc:
- mcdm.monsters.v1:monster:goblin-warrior
scdc:
- 1.1.1:2:304
size: 1S
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '15'
type: monster
---

~~~ds-statblock
name: Goblin Warrior
level: 1
roles:
  - Horde Harrier
ancestry:
  - Goblin
  - Humanoid
ev: "3"
stamina: "15"
speed: 6
movement: Climb
size: 1S
stability: 0
free_strike: 1
might: -2
agility: 2
reason: 0
intuition: 0
presence: -1
traits:
  - name: Crafty
    effects:
      - effect: The warrior doesn't provoke opportunity attacks by moving
abilities:
  - name: Spear Charge
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 3 damage
        t2: 4 damage
        t3: 5 damage
  - name: Bury the Point
    icon: 🗡
    cost: 2 Malice
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature
    effects:
      - roll: Power Roll + 2
        t1: 5 damage; M < 0 bleeding (save ends)
        t2: 6 damage; M < 1 bleeding (save ends)
        t3: 7 damage; M < 2 bleeding (save ends)
~~~