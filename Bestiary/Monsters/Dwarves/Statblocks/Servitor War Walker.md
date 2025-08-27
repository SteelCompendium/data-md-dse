---
agility: 0
ancestry:
- Dwarf
- Humanoid
ev: '12'
file_basename: Servitor War Walker
file_dpath: Monsters/Dwarves/Statblocks
free_strike: 4
intuition: 0
item_id: servitor-war-walker
item_index: '394'
item_name: Servitor War Walker
level: 1
might: 2
presence: -2
reason: -2
roles:
- Elite Mount
scc:
- mcdm.monsters.v1:monster:servitor-war-walker
scdc:
- 1.1.1:2:394
size: '3'
source: mcdm.monsters.v1
speed: 8
stability: 2
stamina: '60'
type: monster
---

```ds-statblock
name: Servitor War Walker
level: 1
roles:
  - Elite Mount
ancestry:
  - Dwarf
  - Humanoid
ev: "12"
stamina: "60"
speed: 8
movement: Climb
size: "3"
stability: 2
free_strike: 4
might: 2
agility: 0
reason: -2
intuition: 0
presence: -2
traits:
  - name: Cupola
    effects:
      - effect: While riding the war walker, three size 1 allies can occupy the same
          space. Creatures riding the war walker have cover.
  - name: Mobile Prison Harness
    effects:
      - effect: Any restrained or slowed creature who comes adjacent to the war walker
          is automatically restrained (save ends) and takes a bane on power
          rolls. A creature restrained this way moves with the war walker.
abilities:
  - name: Grasping Claws
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        t1: 6 damage
        t2: 9 damage
        t3: 12 damage; M < 2 restrained (save ends)
      - effect: A target already restrained or restrained by this ability is pulled up
          to 3 squares. A target restrained by a dwarf can be force moved by
          this ability. This forced movement doesn't end the restrained
          condition unless the Director determines otherwise.
        name: Effect
  - name: Stunning Blast
    icon: ❇️
    cost: 3 Malice
    keywords:
      - Area
      - Weapon
    type: Maneuver
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        t1: 3 lightning damage; A < 0 slowed (save ends)
        t2: 6 lightning damage; A < 1 slowed (save ends)
        t3: 7 lightning damage; A < 2 slowed (save ends)
```