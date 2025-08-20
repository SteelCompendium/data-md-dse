---
agility: 3
ancestry:
- Goblin
- Hobgoblin
- Humanoid
- Infernal
ev: '14'
file_basename: Hobgoblin Incendiarist
file_dpath: Monsters/Hobgoblins/Statblocks
free_strike: 6
intuition: 2
item_id: hobgoblin-incendiarist
item_index: '188'
item_name: Hobgoblin Incendiarist
level: 5
might: 1
presence: 1
reason: 0
roles:
- Platoon Artillery
scc:
- mcdm.monsters.v1:monster:hobgoblin-incendiarist
scdc:
- 1.1.1:2:188
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '60'
type: monster
---

```ds-statblock
name: Hobgoblin Incendiarist
level: 5
roles:
  - Platoon Artillery
ancestry:
  - Goblin
  - Hobgoblin
  - Humanoid
  - Infernal
ev: "14"
stamina: "60"
immunities:
  - Fire 5
speed: 5
size: 1M
stability: 0
free_strike: 6
might: 1
agility: 3
reason: 0
intuition: 2
presence: 1
traits:
  - name: Raining Cinders
    effects:
      - effect: The ranged free strike of each ally within 3 squares of the incendiarist
          has a distance of 10 and deals fire damage.
  - name: Infernal Ichor
    effects:
      - effect: When the incendiarist is reduced to 0 Stamina, they spray burning blood.
          Each creature adjacent to the incendiarist takes 3 fire damage.
abilities:
  - name: Fire Crossbow
    cost: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        t1: 9 fire damage
        t2: 14 fire damage
        t3: 17 fire damage; A < 3 burning (save ends)
      - effect: A burning creature takes 1d6 fire damage at the start of each of their
          turns. A burning object takes 1d6 fire damage at the end of each
          round.
  - name: Fireball Volley
    cost: 3 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    type: Main action
    distance: 4 cube within 10
    target: Each enemy or object in the area
    effects:
      - roll: Power Roll + 3
        t1: 5 fire damage; A < 1 burning (save ends)
        t2: 9 fire damage; A < 2 burning (save ends)
        t3: 11 fire damage; prone; A < 3 burning (save ends)
      - effect: A burning creature takes 1d6 fire damage at the start of each of their
          turns. A burning object takes 1d6 fire damage at the end of each
          round.
```