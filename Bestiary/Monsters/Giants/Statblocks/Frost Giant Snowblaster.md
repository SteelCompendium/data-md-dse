---
agility: -1
ancestry:
- Frost Giant
- Giant
ev: 10 for four minions
file_basename: Frost Giant Snowblaster
file_dpath: Monsters/Giants/Statblocks
free_strike: 4
intuition: 4
item_id: frost-giant-snowblaster
item_index: '195'
item_name: Frost Giant Snowblaster
level: 8
might: 3
presence: 2
reason: -1
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster:frost-giant-snowblaster
scdc:
- 1.1.1:2:195
size: '4'
source: mcdm.monsters.v1
speed: 7
stability: 5
stamina: '12'
type: monster
---

```ds-statblock
name: Frost Giant Snowblaster
level: 8
roles:
  - Minion Artillery
ancestry:
  - Frost Giant
  - Giant
ev: 10 for four minions
stamina: "12"
immunities:
  - Cold 8
speed: 7
size: "4"
stability: 5
free_strike: 4
with_captain: +3 damage bonus to strikes
might: 3
agility: -1
reason: -1
intuition: 4
presence: 2
traits:
  - name: Kingdom of Isolation
    effects:
      - effect: The snowblaster is surrounded by a snowstorm. Any enemy who starts their
          turn within 2 squares of the snowblaster can't shift.
abilities:
  - name: Slushfall
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 12
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 4
        t1: 4 cold damage
        t2: 7 cold damage
        t3: 9 cold damage; prone
```