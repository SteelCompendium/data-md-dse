---
agility: 1
ancestry:
- Humanoid
- Orc
ev: '8'
file_basename: Orc Terranova
file_dpath: Monsters/Orcs/Statblocks
free_strike: 4
intuition: 1
item_id: orc-terranova
item_index: '130'
item_name: Orc Terranova
level: 2
might: 1
presence: 2
reason: 0
roles:
- Platoon Controller
scc:
- mcdm.monsters.v1:monster:orc-terranova
scdc:
- 1.1.1:2:130
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 2
stamina: '30'
type: monster
---

```ds-statblock
name: Orc Terranova
level: 2
roles:
  - Platoon Controller
ancestry:
  - Humanoid
  - Orc
ev: "8"
stamina: "30"
speed: 6
movement: Burrow
size: 1M
stability: 2
free_strike: 4
might: 1
agility: 1
reason: 0
intuition: 1
presence: 2
traits:
  - name: Seismic Step
    effects:
      - effect: The terranova ignores difficult terrain. Additionally, they don't need
          line of effect to use abilities against creatures touching the ground.
  - name: Relentless
    effects:
      - effect: If the terranova is reduced to 0 Stamina, they can make a free strike
          before dying. If the target of the free strike is reduced to 0
          Stamina, the terranova is reduced to 1 Stamina instead.
abilities:
  - name: Earth Pillar
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 10
    target: Three creatures or objects
    effects:
      - roll: Power Roll + 2
        t1: 6 damage; A < 0 prone and can't stand (save ends)
        t2: 9 damage; A < 1 prone and can't stand (save ends)
        t3: 12 damage; A < 2 prone and can't stand (save ends)
      - effect: Each target must be on the ground, and the ground in each target's space
          rises 1 square.
  - name: Sinkhole
    cost: 3 Malice
    keywords:
      - Area
      - Weapon
    type: Main action
    distance: 3 burst
    target: Each enemy and object in the area
    effects:
      - roll: Power Roll + 2
        t1: 4 damage; M < 0 restrained (save ends)
        t2: 7 damage; M < 1 restrained (save ends)
        t3: 10 damage; M < 2 restrained (save ends)
      - effect: The area is difficult terrain
```