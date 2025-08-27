---
agility: 1
ancestry:
- Humanoid
- Radenwight
ev: '6'
file_basename: Radenwight Bruxer
file_dpath: Monsters/Radenwights/Statblocks
free_strike: 4
intuition: 0
item_id: radenwight-bruxer
item_index: '149'
item_name: Radenwight Bruxer
level: 1
might: 2
presence: 1
reason: -1
roles:
- Platoon Brute
scc:
- mcdm.monsters.v1:monster:radenwight-bruxer
scdc:
- 1.1.1:2:149
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '40'
type: monster
---

```ds-statblock
name: Radenwight Bruxer
level: 1
roles:
  - Platoon Brute
ancestry:
  - Humanoid
  - Radenwight
ev: "6"
stamina: "40"
speed: 5
movement: Climb
size: 1L
stability: 2
free_strike: 4
might: 2
agility: 1
reason: -1
intuition: 0
presence: 1
traits:
  - name: Lockdown
    effects:
      - effect: Any enemy who shifts adjacent to the bruxer has that shif t en d
          Additionally, any enemy adjacent to the bruxer can't shift.
abilities:
  - name: Lockjaw
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
        t1: 6 damage
        t2: 9 damage
        t3: 12 damage; grabbed
      - effect: A target grabbed this way takes 2 damage at the start of each of the
          bruxer's turns.
        name: Effect
  - name: Flurry of Bites
    icon: ❇️
    cost: 3 Malice
    keywords:
      - Area
      - Weapon
    type: Main action
    distance: 1 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        t1: 3 damage; A < 0 bleeding (save ends)
        t2: 5 damage; A < 1 bleeding (save ends)
        t3: 8 damage; A < 2 bleeding (save ends)
  - name: Ready Rodent
    icon: ❗️
    keywords:
      - Melee
      - Weapon
    type: Triggered action
    distance: Melee 1
    target: One creature
    trigger: An ally deals damage to the target.
    effects:
      - effect: The bruxer makes a free strike against the target.
        name: Effect
```