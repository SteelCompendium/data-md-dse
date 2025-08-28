---
agility: 3
ancestry:
- Abyssal
- Demon
ev: 6 for four minions
file_basename: Wobalas
file_dpath: Monsters/Demons/Statblocks
free_strike: 3
intuition: 2
item_id: wobalas
item_index: '255'
item_name: Wobalas
level: 4
might: 1
presence: 1
reason: 1
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster:wobalas
scdc:
- 1.1.1:2:255
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '7'
type: monster
---

~~~ds-statblock
name: Wobalas
level: 4
roles:
  - Minion Artillery
ancestry:
  - Abyssal
  - Demon
ev: 6 for four minions
stamina: "7"
weaknesses:
  - Holy 5
speed: 6
size: 1M
stability: 0
free_strike: 3
with_captain: +2 damage bonus to strikes
might: 1
agility: 3
reason: 1
intuition: 2
presence: 1
traits: []
abilities:
  - name: Despair Bolt
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 20
    target: One creature per minion
    effects:
      - roll: Power Roll + 2
        t1: 3 psychic damage
        t2: 5 psychic damage
        t3: 7 psychic damage
      - effect: The target takes a bane on their next strike. If the target is winded,
          they have a double bane on their next strike instead.
        name: Effect
~~~