---
agility: 3
ancestry:
- Devil
- Hobgoblin
- Infernal
ev: 6 for four minions
file_basename: Grilp
file_dpath: Monsters/Hobgoblins/Statblocks
free_strike: 3
intuition: 1
item_id: grilp
item_index: '180'
item_name: Grilp
level: 4
might: -1
presence: 0
reason: 0
roles:
- Minion Ambusher
scc:
- mcdm.monsters.v1:monster:grilp
scdc:
- 1.1.1:2:180
size: 1T
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '8'
type: monster
---

```ds-statblock
name: Grilp
level: 4
roles:
  - Minion Ambusher
ancestry:
  - Devil
  - Hobgoblin
  - Infernal
ev: 6 for four minions
stamina: "8"
immunities:
  - Fire 2
speed: 7
movement: Fly
size: 1T
stability: 0
free_strike: 3
with_captain: +2 bonus to speed
might: -1
agility: 3
reason: 0
intuition: 1
presence: 0
traits:
  - name: Bat Out Of Hell
    effects:
      - effect: Any enemy who makes a saving throw takes a −1 penalty to the saving
          throw for each grilp adjacent to them.
  - name: Shifting Camouflage
    effects:
      - effect: The grilp has concealment from all creatures.
abilities:
  - name: Flyby Bite
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
        t3: 7 damage; the grilp shifts up to 2 squares
      - effect: The grilp moves up to their speed and can attempt to hide.
```