---
agility: 5
ancestry:
- Abyssal
- Demon
ev: 12 for four minions
file_basename: Tyburaki
file_dpath: Monsters/Demons/Statblocks
free_strike: 4
intuition: 3
item_id: tyburaki
item_index: '259'
item_name: Tyburaki
level: 10
might: 2
presence: -1
reason: 0
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster:tyburaki
scdc:
- 1.1.1:2:259
size: '2'
source: mcdm.monsters.v1
speed: 8
stability: 0
stamina: '15'
type: monster
---

~~~ds-statblock
name: Tyburaki
level: 10
roles:
  - Minion Harrier
ancestry:
  - Abyssal
  - Demon
ev: 12 for four minions
stamina: "15"
weaknesses:
  - Holy 5
speed: 8
movement: Swim
size: "2"
stability: 0
free_strike: 4
with_captain: +4 damage bonus to strikes
might: 2
agility: 5
reason: 0
intuition: 3
presence: -1
traits:
  - name: Breacher
    effects:
      - effect: While swimming, the tyburaki can jump 5 squares as part of their
          movement.
  - name: Soulsight
    effects:
      - effect: Any creature within 2 squares of the tyburaki can't be hidden from them.
abilities:
  - name: Tail Bite
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 3
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 5
        t1: 4 damage
        t2: 7 damage
        t3: 9 damage
      - effect: The tyburaki can make a free strike against each enemy adjacent to the
          target.
        name: Effect
~~~