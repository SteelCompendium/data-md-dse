---
agility: 2
ancestry:
- Fey
- High Elf
- Humanoid
ev: '6'
file_basename: High Elf Zephyr
file_dpath: Monsters/Elves High/Statblocks
free_strike: 3
intuition: 0
item_id: high-elf-zephyr
item_index: '119'
item_name: High Elf Zephyr
level: 1
might: 0
presence: 1
reason: 0
roles:
- Platoon Harrier
scc:
- mcdm.monsters.v1:monster:high-elf-zephyr
scdc:
- 1.1.1:2:119
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '30'
type: monster
---

```ds-statblock
name: High Elf Zephyr
level: 1
roles:
  - Platoon Harrier
ancestry:
  - Fey
  - High Elf
  - Humanoid
ev: "6"
stamina: "30"
speed: 7
size: 1M
stability: 0
free_strike: 3
might: 0
agility: 2
reason: 0
intuition: 0
presence: 1
traits:
  - name: Like the Wind
    effects:
      - effect: The zephyr doesn't provoke opportunity attacks by moving.
  - name: Otherworldly Grace
    effects:
      - effect: At the start of each of their turns, the zephyr can choose one effect on
          them that can be ended by a saving throw. That effect instead ends at
          the end of their turn.
abilities:
  - name: Sweeping Blade
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 5 damage
        t2: 7 damage
        t3: 9 damage
      - effect: On a tier 3 outcome, the zephyr can make a free strike against a
          creature adjacent to the target. If they do so and that creature and
          the target both have A < 2, the creature and the target are both
          prone. On any tier outcome, the zephyr can then shift up to 2 squares
        name: Effect
  - name: Windwalk
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The zephyr flies up to their speed. If they don't end this movment on
          solid ground, they are prone.
        name: Effect
```