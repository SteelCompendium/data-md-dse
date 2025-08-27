---
agility: 2
ancestry:
- Goblin
- Hobgoblin
- Humanoid
- Infernal
ev: '12'
file_basename: Hobgoblin Hell Trooper
file_dpath: Monsters/Hobgoblins/Statblocks
free_strike: 6
intuition: 0
item_id: hobgoblin-hell-trooper
item_index: '179'
item_name: Hobgoblin Hell Trooper
level: 4
might: 3
presence: 1
reason: 0
roles:
- Platoon Brute
scc:
- mcdm.monsters.v1:monster:hobgoblin-hell-trooper
scdc:
- 1.1.1:2:179
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '70'
type: monster
---

```ds-statblock
name: Hobgoblin Hell Trooper
level: 4
roles:
  - Platoon Brute
ancestry:
  - Goblin
  - Hobgoblin
  - Humanoid
  - Infernal
ev: "12"
stamina: "70"
immunities:
  - Fire 4
speed: 5
size: 1M
stability: 2
free_strike: 6
might: 3
agility: 2
reason: 0
intuition: 0
presence: 1
traits:
  - name: Infernal Ichor
    effects:
      - effect: When the trooper is reduced to 0 Stamina, they spray burning blood. Each
          creature adjacent to the trooper takes 3 fire damage.
abilities:
  - name: Fire Flail
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        t1: 7 fire damage
        t2: 10 fire damage
        t3: 13 fire damage
      - effect: Until the end of their turn, the trooper doesn't provoke opportunity
          attacks from any target.
        name: Effect
  - name: Fight Me, Coward!
    icon: 🏹
    keywords:
      - Magic
      - Ranged
    type: Maneuver
    distance: Ranged 5
    target: One creature
    effects:
      - effect: If the target has P < 2, they are taunted (EoT). While taunted this way,
          the target takes 1d6 fire damage whenever they use an ability or
          strike that doesn't target the trooper.
        name: Effect
```