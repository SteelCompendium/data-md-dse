---
agility: 2
ancestry:
- Abyssal
- Demon
ev: '7'
file_basename: Fiktin
file_dpath: Monsters/Demons/Statblocks
free_strike: 3
intuition: 1
item_id: fiktin
item_index: '265'
item_name: Fiktin
level: 5
might: 2
presence: 3
reason: 2
roles:
- Horde Ambusher
scc:
- mcdm.monsters.v1:monster:fiktin
scdc:
- 1.1.1:2:265
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '35'
type: monster
---

~~~ds-statblock
name: Fiktin
level: 5
roles:
  - Horde Ambusher
ancestry:
  - Abyssal
  - Demon
ev: "7"
stamina: "35"
weaknesses:
  - Holy 5
speed: 6
size: 1M
stability: 0
free_strike: 3
might: 2
agility: 2
reason: 2
intuition: 1
presence: 3
traits:
  - name: Lethe
    effects:
      - effect: While the fiktin is winded, they gain an edge on strikes, and any strike
          made against them gains an edge.
  - name: Soulsight
    effects:
      - effect: Any creature within 2 squares of the fiktin can't be hidden from them.
abilities:
  - name: Violent Transformation
    icon: ❇️
    cost: Signature Ability
    keywords:
      - Area
      - Magic
    type: Main action
    distance: 2 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        t1: 3 corruption damage
        t2: 6 corruption damage
        t3: 7 corruption damage; I < 3 dazed (save ends)
      - effect: The fiktin violently changes shape, dealing an extra 6 damage to any
          target they were hidden from with their Aggressive Mimicry ability.
        name: Effect
  - name: Aggressive Mimicry
    icon: 👤
    cost: 1 Malice
    keywords:
      - Magic
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The fiktin transforms into a mundane object of their size or smaller and
          is automatically hidden. They can revert to their true form as a free
          maneuver.
        name: Effect
~~~