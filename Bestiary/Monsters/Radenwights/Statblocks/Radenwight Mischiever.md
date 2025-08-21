---
agility: 2
ancestry:
- Humanoid
- Radenwight
ev: 3 for 4 minions
file_basename: Radenwight Mischiever
file_dpath: Monsters/Radenwights/Statblocks
free_strike: 2
intuition: 1
item_id: radenwight-mischiever
item_index: '153'
item_name: Radenwight Mischiever
level: 1
might: -1
presence: 0
reason: 0
roles:
- Minion Ambusher
scc:
- mcdm.monsters.v1:monster:radenwight-mischiever
scdc:
- 1.1.1:2:153
size: 1S
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '4'
type: monster
---

```ds-statblock
name: Radenwight Mischiever
level: 1
roles:
  - Minion Ambusher
ancestry:
  - Humanoid
  - Radenwight
ev: 3 for 4 minions
stamina: "4"
speed: 7
movement: Climb
size: 1S
stability: 0
free_strike: 2
with_captain: +1 damage bonus to strikes
might: -1
agility: 2
reason: 0
intuition: 1
presence: 0
traits: []
abilities:
  - name: Dagger Dance
    cost: Signature Ability
    keywords:
      - Melee
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1 or ranged 5
    target: One creature per minion
    effects:
      - roll: Power Roll + 2
        t1: 2 damage
        t2: 4 damage
        t3: 5 damage
      - effect: If the mischiever is hidden when they use this ability, they can target
          two creatures.
        name: Effect
  - name: Ready Rodent
    keywords:
      - Melee
      - Weapon
    type: Triggered action
    distance: Melee 1
    target: One creature
    trigger: An ally deals damage to the target.
    effects:
      - effect: The mischiever makes a free strike against the target.
        name: Effect
```