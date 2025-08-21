---
agility: 2
ancestry:
- Animal
- Orc
ev: 3 for four minions
file_basename: Mohler
file_dpath: Monsters/Orcs/Statblocks
free_strike: 2
intuition: 1
item_id: mohler
item_index: '123'
item_name: Mohler
level: 1
might: 0
presence: -3
reason: -4
roles:
- Minion Ambusher
scc:
- mcdm.monsters.v1:monster:mohler
scdc:
- 1.1.1:2:123
size: 1S
source: mcdm.monsters.v1
speed: 7
stability: 1
stamina: '4'
type: monster
---

```ds-statblock
name: Mohler
level: 1
roles:
  - Minion Ambusher
ancestry:
  - Animal
  - Orc
ev: 3 for four minions
stamina: "4"
speed: 7
movement: Burrow
size: 1S
stability: 1
free_strike: 2
with_captain: +2 bonus to speed
might: 0
agility: 2
reason: -4
intuition: 1
presence: -3
traits:
  - name: Seismic Sense
    effects:
      - effect: The mohler doesn't need line of effect to use abilities against
          creatures or objects touching the ground.
  - name: Ground Grinder
    effects:
      - effect: The mohler can use the Dig maneuver at the start of the encounter.
          Additionally, while the mohler burrows within 1 square below the
          ground, the ground above where they burrow is difficult terrain.
abilities:
  - name: Earth Bump
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        t1: 2 damage
        t2: 4 damage
        t3: 5 damage
      - effect: The distance increases to melee 2. If the mohler is 1 or more squares
          beneath the target before they use this ability, a target who has M <
          1 is also knocked prone.
        name: Effect
```