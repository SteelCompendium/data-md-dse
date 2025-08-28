---
agility: 0
ancestry:
- Abyssal
- Gnoll
ev: 4 for four minions
file_basename: Gnoll Chainflai
file_dpath: Monsters/Gnolls/Statblocks
free_strike: 3
intuition: 0
item_id: gnoll-chainflai
item_index: '43'
item_name: Gnoll Chainflai
level: 2
might: 2
presence: -2
reason: 1
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster:gnoll-chainflai
scdc:
- 1.1.1:2:43
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '4'
type: monster
---

~~~ds-statblock
name: Gnoll Chainflai
level: 2
roles:
  - Minion Artillery
ancestry:
  - Abyssal
  - Gnoll
ev: 4 for four minions
stamina: "4"
speed: 5
size: 1M
stability: 1
free_strike: 3
with_captain: +1 damage bonus to strikes
might: 2
agility: 0
reason: 1
intuition: 0
presence: -2
traits:
  - name: Death Circle
    effects:
      - effect: Whenever a non-minion ally within 5 squares of the chainflail is reduced
          to 0 Stamina, the chainflail can move up to their speed.
abilities:
  - name: Chain Shotput
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 8
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        t1: 3 damage
        t2: 4 damage; push 1
        t3: 6 damage; push 3
~~~