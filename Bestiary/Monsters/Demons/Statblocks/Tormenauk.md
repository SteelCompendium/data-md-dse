---
agility: 0
ancestry:
- Abyssal
- Demon
ev: '8'
file_basename: Tormenauk
file_dpath: Monsters/Demons/Statblocks
free_strike: 4
intuition: 1
item_id: tormenauk
item_index: '281'
item_name: Tormenauk
level: 6
might: 3
presence: 2
reason: 2
roles:
- Horde Brute
scc:
- mcdm.monsters.v1:monster:tormenauk
scdc:
- 1.1.1:2:281
size: '2'
source: mcdm.monsters.v1
speed: 6
stability: 2
stamina: '45'
type: monster
---

```ds-statblock
name: Tormenauk
level: 6
roles:
  - Horde Brute
ancestry:
  - Abyssal
  - Demon
ev: "8"
stamina: "45"
weaknesses:
  - Holy 5
speed: 6
size: "2"
stability: 2
free_strike: 4
might: 3
agility: 0
reason: 2
intuition: 1
presence: 2
traits:
  - name: Lethe
    effects:
      - effect: While the tormenauk is winded, they gain an edge on strikes, and any
          strike made against them gains an edge.
  - name: Soulsight
    effects:
      - effect: Any creature within 2 squares of the tormenauk can't be hidden from
          them.
abilities:
  - name: Many Maws
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        t1: 7 damage
        t2: 9 damage
        t3: 11 damage; grabbed, and the target takes a bane on the Escape Grab maneuver
      - effect: Any target grabbed this way takes 4 psychic damage at the start of each
          of the tormenauk's turns.
        name: Effect
  - name: Agony Wail
    cost: 5 Malice
    keywords:
      - Area
      - Magic
    type: Maneuver
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        t1: 4 psychic damage; I < 1 dazed (save ends)
        t2: 6 psychic damage; I < 2 dazed (save ends)
        t3: 8 psychic damage; I < 3 dazed (save ends)
      - effect: The potency increases by 1 if the target is grabbed by the tormenauk.
        name: Effect
```