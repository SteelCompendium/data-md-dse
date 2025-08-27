---
agility: 2
ancestry:
- Goblin
- Hobgoblin
- Humanoid
- Infernal
ev: 6 for four minions
file_basename: Hobgoblin Recruit
file_dpath: Monsters/Hobgoblins/Statblocks
free_strike: 3
intuition: 0
item_id: hobgoblin-recruit
item_index: '177'
item_name: Hobgoblin Recruit
level: 4
might: 3
presence: 1
reason: 0
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster:hobgoblin-recruit
scdc:
- 1.1.1:2:177
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '9'
type: monster
---

```ds-statblock
name: Hobgoblin Recruit
level: 4
roles:
  - Minion Brute
ancestry:
  - Goblin
  - Hobgoblin
  - Humanoid
  - Infernal
ev: 6 for four minions
stamina: "9"
immunities:
  - Fire 2
speed: 5
size: 1M
stability: 0
free_strike: 3
with_captain: +4 bonus to Stamina
might: 3
agility: 2
reason: 0
intuition: 0
presence: 1
traits:
  - name: Tactical Positioning
    effects:
      - effect: Any non-minion ally deals 1 extra damage for each recruit adjacent to
          them.
  - name: Infernal Ichor
    effects:
      - effect: When the recruit is reduced to 0 Stamina, they spray burning blood. Each
          creature adjacent to the recruit takes 2 fire damage.
abilities:
  - name: Sword Lunge
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 3
        t1: 3 damage
        t2: 5 damage
        t3: 7 damage; grabbed or prone
```