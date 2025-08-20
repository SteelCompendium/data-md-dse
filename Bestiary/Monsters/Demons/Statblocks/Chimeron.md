---
agility: 0
ancestry:
- Abyssal
- Demon
ev: '9'
file_basename: Chimeron
file_dpath: Monsters/Demons/Statblocks
free_strike: 5
intuition: 1
item_id: chimeron
item_index: '268'
item_name: Chimeron
level: 9
might: 4
presence: 2
reason: 2
roles:
- Horde Brute
scc:
- mcdm.monsters.v1:monster:chimeron
scdc:
- 1.1.1:2:268
size: '3'
source: mcdm.monsters.v1
speed: 6
stability: 2
stamina: '90'
type: monster
---

```ds-statblock
name: Chimeron
level: 9
roles:
  - Horde Brute
ancestry:
  - Abyssal
  - Demon
ev: "9"
stamina: "90"
weaknesses:
  - Holy 5
speed: 6
size: "3"
stability: 2
free_strike: 5
might: 4
agility: 0
reason: 2
intuition: 1
presence: 2
traits:
  - name: Lethe
    effects:
      - effect: While the chimeron is winded, they gain an edge on strikes, and any
          strike made against them gains an edge.
  - name: Soulsight
    effects:
      - effect: Any creature within 2 squares of the chimeron can't be hidden from them.
abilities:
  - name: Flux Gnash
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        t1: 9 cold, fire, or sonic damage
        t2: 11 cold, fire, or sonic damage
        t3: 13 cold, fire, or sonic damage; M < 4 bleeding, dazed, or slowed (save ends)
      - effect: After making the power roll, the chimeron decides what damage type the
          ability deals and which condition it imposes.
        name: Special
  - name: Pain Absorption
    cost: 1 Malice
    keywords:
      - "-"
    type: Triggered action
    distance: Self
    target: Self
    trigger: The chimeron is targeted by a damage-dealing strike.
    effects:
      - effect: The chimeron halves the damage.
```