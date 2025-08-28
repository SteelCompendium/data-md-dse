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
traits:
  - name: Lethe
    effects:
      - effect: While the izyak is winded, they gain an edge on strikes, and any strike
          made against them gains an edge.
  - name: Soulsight
    effects:
      - effect: Any creature within 2 squares of the izyak can't be hidden from them.
abilities:
  - name: Nostalgic Wanderlust
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Psionic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 10
    target: One creature
    effects:
      - roll: Power Roll + 5
        t1: 9 psychic damage; R < 3 restrained (save ends)
        t2: 12 psychic damage; R < 4 restrained (save ends)
        t3: 14 psychic damage; R < 5 restrained (save ends)
      - effect: The izyak can slide any target restrained this way up to 3 squares.
        name: Effect
      - effect: The izyak can vertical slide any target restrained this way up to 6
          squares instead. A target left in midair doesn't fall until the
          restrained condition ends.
        cost: 3 Malice
  - name: Ruinous Temptation
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
      - Psionic
      - Ranged
    type: Main action
    distance: 4 cube within 10
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 5
        t1: 4 psychic damage; I < 3 dazed (save ends)
        t2: 7 psychic damage; I < 4 dazed (save ends)
        t3: 9 psychic damage; I < 5 dazed (save ends)
      - effect: Any target dazed this way must use a move action to move their speed
          toward the izyak on their next turn.
        name: Effect
      - effect: The area increases to a 6 cube.
        cost: 2 Malice
~~~