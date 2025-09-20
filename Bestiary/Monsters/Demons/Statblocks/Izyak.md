---
agility: 0
ancestry:
- Abyssal
- Demon
ev: '12'
file_basename: Izyak
file_dpath: Monsters/Demons/Statblocks
free_strike: 4
intuition: 2
item_id: izyak
item_index: '271'
item_name: Izyak
level: 10
might: 0
presence: 4
reason: 5
roles:
- Horde Controller
scc:
- mcdm.monsters.v1:monster:izyak
scdc:
- 1.1.1:2:271
size: '2'
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '55'
type: monster
---

~~~ds-statblock
type: statblock
name: Izyak
level: 10
roles:
  - Horde Controller
ancestry:
  - Abyssal
  - Demon
ev: "12"
stamina: "55"
weaknesses:
  - Holy 5
speed: 6
movement: Teleport
size: "2"
stability: 0
free_strike: 4
might: 0
agility: 0
reason: 5
intuition: 2
presence: 4
features:
  - type: feature
    feature_type: ability
    name: Nostalgic Wanderlust
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Psionic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 10
    target: One creature
    effects:
      - roll: Power Roll + 5
        tier1: 9 psychic damage; R < 3 restrained (save ends)
        tier2: 12 psychic damage; R < 4 restrained (save ends)
        tier3: 14 psychic damage; R < 5 restrained (save ends)
      - name: Effect
        effect: The izyak can slide any target restrained this way up to 3 squares.
      - cost: 3 Malice
        effect: The izyak can vertical slide any target restrained this way up to 6
          squares instead. A target left in midair doesn't fall until the
          restrained condition ends.
  - type: feature
    feature_type: ability
    name: Ruinous Temptation
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
      - Psionic
      - Ranged
    usage: Main action
    distance: 4 cube within 10
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 5
        tier1: 4 psychic damage; I < 3 dazed (save ends)
        tier2: 7 psychic damage; I < 4 dazed (save ends)
        tier3: 9 psychic damage; I < 5 dazed (save ends)
      - name: Effect
        effect: Any target dazed this way must use a move action to move their speed
          toward the izyak on their next turn.
      - cost: 2 Malice
        effect: The area increases to a 6 cube.
  - type: feature
    feature_type: trait
    name: Lethe
    icon: ⭐️
    effects:
      - effect: While the izyak is winded, they gain an edge on strikes, and any strike
          made against them gains an edge.
  - type: feature
    feature_type: trait
    name: Soulsight
    icon: ⭐️
    effects:
      - effect: Any creature within 2 squares of the izyak can't be hidden from them.
~~~