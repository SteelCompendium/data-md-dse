---
agility: 5
ancestry:
- Abyssal
- Demon
ev: 12 for four minions
file_basename: Unguloid
file_dpath: Monsters/Demons/Statblocks
free_strike: 5
intuition: -1
item_id: unguloid
item_index: '254'
item_name: Unguloid
level: 10
might: 5
presence: -1
reason: -1
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster:unguloid
scdc:
- 1.1.1:2:254
size: '2'
source: mcdm.monsters.v1
speed: 8
stability: 3
stamina: '17'
type: monster
---

~~~ds-statblock
name: Unguloid
level: 10
roles:
  - Minion Brute
ancestry:
  - Abyssal
  - Demon
ev: 12 for four minions
stamina: "17"
weaknesses:
  - Holy 5
speed: 8
size: "2"
stability: 3
free_strike: 5
with_captain: Have a double edge on strikes
might: 5
agility: 5
reason: -1
intuition: -1
presence: -1
traits:
  - name: Soulsight
    effects:
      - effect: Any creature within 2 squares of the unguloid can't be hidden from them.
abilities:
  - name: Gore Horn
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 5
        t1: 5 damage; push 2
        t2: 8 damage; push 4
        t3: 10 damage; push 6
      - effect: If this ability is used as part of a charge for which the unguloid moves
          2 squares or more, it deals an extra 10 damage.
        name: Effect
~~~