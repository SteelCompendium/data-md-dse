---
agility: 3
ancestry:
- Goblin
- Hobgoblin
- Humanoid
- Infernal
ev: '14'
file_basename: Hobgoblin Smokebinder
file_dpath: Monsters/Hobgoblins/Statblocks
free_strike: 6
intuition: 1
item_id: hobgoblin-smokebinder
item_index: '181'
item_name: Hobgoblin Smokebinder
level: 5
might: 1
presence: 0
reason: 2
roles:
- Platoon Ambusher
scc:
- mcdm.monsters.v1:monster:hobgoblin-smokebinder
scdc:
- 1.1.1:2:181
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '70'
type: monster
---

```ds-statblock
name: Hobgoblin Smokebinder
level: 5
roles:
  - Platoon Ambusher
ancestry:
  - Goblin
  - Hobgoblin
  - Humanoid
  - Infernal
ev: "14"
stamina: "70"
immunities:
  - Fire 5
speed: 7
movement: Fly, hover
size: 1M
stability: 0
free_strike: 6
might: 1
agility: 3
reason: 2
intuition: 1
presence: 0
traits:
  - name: Essence of Smoke
    effects:
      - effect: The smokebinder can move through spaces as if they were size 1T and can
          occupy another creature or object's space. At the end of their turn,
          the smokebinder can attempt to hide if they haven't taken any damage
          since their last turn.
  - name: Infernal Ichor
    effects:
      - effect: When the smokebinder is reduced to 0 Stamina, they spray burning blood.
          Each creature adjacent to the smokebinder takes 3 fire damage.
abilities:
  - name: Choking Bolt
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 5
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        t1: 9 fire damage
        t2: 14 fire damage
        t3: 17 fire damage; R < 3 slowed (save ends)
      - effect: If this ability gains an edge or has a double edge, the target can't
          communicate with anyone until the end of their next turn.
  - name: Smoke Bomb
    cost: 3 Malice
    keywords:
      - Area
      - Magic
    type: Maneuver
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - effect: >-
          Each target makes a Might test.

          - **≤11:** 11 damage; the target has a double bane on their next power
          roll

          - **12-16:** 9 damage; the target takes a bane on their next power
          roll

          - **17+:** 5 damage
```