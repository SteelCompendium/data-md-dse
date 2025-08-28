---
agility: 2
ancestry:
- Angulotl
ev: 3 for 4 minions
file_basename: Angulotl Pollywog
file_dpath: Monsters/Angulotls/Statblocks
free_strike: 1
intuition: -2
item_id: angulotl-pollywog
item_index: '242'
item_name: Angulotl Pollywog
level: 1
might: 0
presence: 0
reason: -2
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster:angulotl-pollywog
scdc:
- 1.1.1:2:242
size: 1S
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '4'
type: monster
---

~~~ds-statblock
name: Angulotl Pollywog
level: 1
roles:
  - Minion Harrier
ancestry:
  - Angulotl
ev: 3 for 4 minions
stamina: "4"
immunities:
  - Poison 2
speed: 6
movement: Climb, swim
size: 1S
stability: 0
free_strike: 1
with_captain: +2 bonus to speed
might: 0
agility: 2
reason: -2
intuition: -2
presence: 0
traits:
  - name: Quick Snack
    effects:
      - effect: Any angulotl who can target the pollywog with a melee free strike can
          eat them as a maneuver. The angulotl regains 4 Stamina and is wet
          until the end of their next turn.
abilities:
  - name: Nip
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
        t3: 3 poison damage; the pollywog shifts up to 3 squares
~~~