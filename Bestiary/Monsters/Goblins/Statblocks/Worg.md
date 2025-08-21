---
agility: 2
ancestry:
- Animal
- Goblin
ev: '3'
file_basename: Worg
file_dpath: Monsters/Goblins/Statblocks
free_strike: 1
intuition: 0
item_id: worg
item_index: '306'
item_name: Worg
level: 1
might: 1
presence: -1
reason: -1
roles:
- Horde Mount
scc:
- mcdm.monsters.v1:monster:worg
scdc:
- 1.1.1:2:306
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '15'
type: monster
---

```ds-statblock
name: Worg
level: 1
roles:
  - Horde Mount
ancestry:
  - Animal
  - Goblin
ev: "3"
stamina: "15"
speed: 5
size: 1L
stability: 1
free_strike: 1
might: 1
agility: 2
reason: -1
intuition: 0
presence: -1
traits:
  - name: Mounted Charger
    effects:
      - effect: If a worg used as a mount charges, their rider gains an edge on melee
          strikes until the end of the rider's turn.
  - name: Shared Craft
    effects:
      - effect: If the worg's rider has the Crafty trait, the worg also has that trait.
abilities:
  - name: Bite
    cost: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 3 damage
        t2: 4 damage
        t3: 5 damage
  - name: Sprint
    cost: 1 Malice
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The worg moves up to their speed.
        name: Effect
```