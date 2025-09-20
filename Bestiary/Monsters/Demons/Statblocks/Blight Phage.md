---
agility: 0
ancestry:
- Abyssal
- Demon
ev: '9'
file_basename: Blight Phage
file_dpath: Monsters/Demons/Statblocks
free_strike: 3
intuition: 2
item_id: blight-phage
item_index: '283'
item_name: Blight Phage
level: 7
might: 0
presence: 4
reason: 4
roles:
- Horde Controller
scc:
- mcdm.monsters.v1:monster:blight-phage
scdc:
- 1.1.1:2:283
size: '3'
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '40'
type: monster
---

~~~ds-statblock
type: statblock
name: Blight Phage
level: 7
roles:
  - Horde Controller
ancestry:
  - Abyssal
  - Demon
ev: "9"
stamina: "40"
weaknesses:
  - Holy 5
speed: 6
size: "3"
stability: 0
free_strike: 3
might: 0
agility: 0
reason: 4
intuition: 2
presence: 4
features:
  - type: feature
    feature_type: ability
    name: Blight Pus
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        tier1: 7 corruption damage
        tier2: 10 corruption damage
        tier3: 11 corruption damage
      - name: Effect
        effect: A puddle of blight-digested soul juice-covers the ground in the target's
          square, which is affected as if by Seeping Blight (see the Level 7+
          Demon Malice feature).
  - type: feature
    feature_type: ability
    name: Blight Rain
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
      - Magic
    usage: Maneuver
    distance: 5 cube within 1
    target: Each enemy in the area
    effects:
      - name: Special
        effect: The blight phage must create the cube beneath themself.
      - name: Effect
        effect: The blight phage spins and sheds corruptive blight to fill the area,
          which is treated as if affected by Seeping Blight.
      - cost: 2 Malice
        effect: The blight phage chooses three 2 cube areas within 10 squares of the
          phage. Each area is covered with blight and treated as if affected by
          Seeping Blight.
  - type: feature
    feature_type: trait
    name: Lethe
    icon: ⭐️
    effects:
      - effect: While the blight phage is winded, they gain an edge on strikes, and any
          strike made against them gains an edge.
  - type: feature
    feature_type: trait
    name: Soulsight
    icon: ⭐️
    effects:
      - effect: Any creature within 2 squares of the blight phage can't be hidden from
          them.
~~~