---
agility: 0
ancestry:
- Goblin
- Hobgoblin
- Humanoid
- Infernal
ev: '12'
file_basename: Hobgoblin Death Captain
file_dpath: Monsters/Hobgoblins/Statblocks
free_strike: 5
intuition: 0
item_id: hobgoblin-death-captain
item_index: '189'
item_name: Hobgoblin Death Captain
level: 4
might: 3
presence: 2
reason: 1
roles:
- Platoon Support
scc:
- mcdm.monsters.v1:monster:hobgoblin-death-captain
scdc:
- 1.1.1:2:189
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '60'
type: monster
---

```ds-statblock
name: Hobgoblin Death Captain
level: 4
roles:
  - Platoon Support
ancestry:
  - Goblin
  - Hobgoblin
  - Humanoid
  - Infernal
ev: "12"
stamina: "60"
immunities:
  - Fire 4
speed: 5
size: 1M
stability: 2
free_strike: 5
might: 3
agility: 0
reason: 1
intuition: 0
presence: 2
traits:
  - name: Battle Ready
    effects:
      - effect: Any hidden creature who makes a strike against the death captain or any
          ally within 2 squares of the death captain takes a bane on the strike.
  - name: Infernal Ichor
    effects:
      - effect: When the death captain is reduced to 0 Stamina, they spray burning
          blood. Each creature adjacent to the death captain takes 3 fire
          damage.
abilities:
  - name: Blightblade
    cost: Signature Ability
    keywords:
      - Magic
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        t1: 8 damage
        t2: 8 damage, 4 corruption damage
        t3: 8 damage, 7 corruption damage
      - effect: The next strike made against the target has a double edge.
      - effect: One ally adjacent to the target can use their signature ability.
        cost: 3 Malice
  - name: On My Mark!
    keywords:
      - Ranged
    type: Maneuver
    distance: Ranged 5
    target: One ally
    effects:
      - effect: The target moves up to their speed and can make a free strike.
```