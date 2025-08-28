---
agility: 2
ancestry:
- Animal
- Goblin
ev: 3 for four minions
file_basename: Skitterling
file_dpath: Monsters/Goblins/Statblocks
free_strike: 1
intuition: 0
item_id: skitterling
item_index: '310'
item_name: Skitterling
level: 1
might: -5
presence: -2
reason: -4
roles:
- Minion Hexer
scc:
- mcdm.monsters.v1:monster:skitterling
scdc:
- 1.1.1:2:310
size: 1T
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '3'
type: monster
---

~~~ds-statblock
name: Skitterling
level: 1
roles:
  - Minion Hexer
ancestry:
  - Animal
  - Goblin
ev: 3 for four minions
stamina: "3"
speed: 5
movement: Fly
size: 1T
stability: 0
free_strike: 1
with_captain: +3 bonus to speed
might: -5
agility: 2
reason: -4
intuition: 0
presence: -2
traits: []
abilities:
  - name: Claws
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature per minion
    effects:
      - roll: Power Roll + 2
        t1: 1 poison damage
        t2: 2 poison damage
        t3: 3 poison damage
      - effect: The target takes a bane on their next strike.
        name: Effect
~~~