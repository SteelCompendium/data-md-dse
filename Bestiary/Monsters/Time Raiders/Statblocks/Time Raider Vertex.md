---
agility: 1
ancestry:
- Humanoid
- Time Raider
ev: '10'
file_basename: Time Raider Vertex
file_dpath: Monsters/Time Raiders/Statblocks
free_strike: 5
intuition: 1
item_id: time-raider-vertex
item_index: '146'
item_name: Time Raider Vertex
level: 3
might: 1
presence: 0
reason: 2
roles:
- Platoon Support
scc:
- mcdm.monsters.v1:monster:time-raider-vertex
scdc:
- 1.1.1:2:146
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '62'
type: monster
---

```ds-statblock
name: Time Raider Vertex
level: 3
roles:
  - Platoon Support
ancestry:
  - Humanoid
  - Time Raider
ev: "10"
stamina: "62"
immunities:
  - Psychic 3
speed: 5
movement: Fly, hover
size: "2"
stability: 2
free_strike: 5
might: 1
agility: 1
reason: 2
intuition: 1
presence: 0
traits:
  - name: Foresight
    effects:
      - effect: The vertex doesn't take a bane on strikes against creatures with
          concealment.
abilities:
  - name: Psionic Slam
    cost: Signature Ability
    keywords:
      - Melee
      - Psionic
      - Strike
    type: Main action
    distance: Melee 2
    target: One creature
    effects:
      - roll: Power Roll + 2
        t1: 5 damage, 2 psychic damage
        t2: 7 damage, 3 psychic damage
        t3: 9 damage, 4 psychic damage
      - effect: Any power roll made against the target gains an edge until the start of
          the vertex's next turn.
  - name: Split Space
    cost: 5 Malice
    keywords:
      - Area
      - Psionic
      - Ranged
    type: Main action
    distance: 2 cube within 10
    target: Special
    effects:
      - effect: A portal fills the area, connecting to a location the vertex has
          experienced on any plane of existence, in person or otherwise. Any
          creature who enters the portal for the first time in a round or starts
          their turn there is instantly teleported to any unoccupied space in
          the portal at the chosen location. The portal lasts until the vertex
          uses this ability again, dismisses the portal (no action required), or
          is transported by the portal.
  - name: Invigorated March
    keywords:
      - Area
      - Psionic
    type: Maneuver
    distance: 4 burst
    target: Each ally in the area
    effects:
      - effect: Each target shifts up to half their speed.
```