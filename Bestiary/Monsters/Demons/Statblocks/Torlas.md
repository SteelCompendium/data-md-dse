---
agility: 1
ancestry:
- Abyssal
- Demon
ev: '3'
file_basename: Torlas
file_dpath: Monsters/Demons/Statblocks
free_strike: 1
intuition: 0
item_id: torlas
item_index: '286'
item_name: Torlas
level: 1
might: 0
presence: 2
reason: 0
roles:
- Horde Controller
scc:
- mcdm.monsters.v1:monster:torlas
scdc:
- 1.1.1:2:286
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '10'
type: monster
---

```ds-statblock
name: Torlas
level: 1
roles:
  - Horde Controller
ancestry:
  - Abyssal
  - Demon
ev: "3"
stamina: "10"
weaknesses:
  - Holy 3
speed: 5
size: 1S
stability: 0
free_strike: 1
might: 0
agility: 1
reason: 0
intuition: 0
presence: 2
traits:
  - name: Lethe
    effects:
      - effect: While the torlas is winded, they gain an edge on strikes, and any strike
          made against them gains an edge.
  - name: Soulsight
    effects:
      - effect: Any creature within 2 squares of the torlas can't be hidden from them.
abilities:
  - name: Floor to Flesh
    cost: Signature Ability
    keywords:
      - Area
      - Magic
      - Ranged
    type: Main action
    distance: 3 cube within 10
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        t1: Slide 3
        t2: Slide 4
        t3: Slide 5
      - effect: The ground in the area turns into a morass of spongy flesh before the
          targets are force moved. Until the start of the torlas's next turn,
          the area is difficult terrain, and each creature who moves in the area
          takes 1 damage for each square moved.
  - name: Grasping Tendons
    keywords:
      - Magic
      - Ranged
    type: Maneuver
    distance: Ranged 10
    target: Three creatures
    effects:
      - effect: The torlas pulls each target up to 3 squares.
```