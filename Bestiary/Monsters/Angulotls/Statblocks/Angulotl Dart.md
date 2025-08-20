---
agility: 2
ancestry:
- Angulotl
- Humanoid
ev: 3 for 4 minions
file_basename: Angulotl Dart
file_dpath: Monsters/Angulotls/Statblocks
free_strike: 2
intuition: 0
item_id: angulotl-dart
item_index: '239'
item_name: Angulotl Dart
level: 1
might: 0
presence: 0
reason: 1
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster:angulotl-dart
scdc:
- 1.1.1:2:239
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '3'
type: monster
---

```ds-statblock
name: Angulotl Dart
level: 1
roles:
  - Minion Artillery
ancestry:
  - Angulotl
  - Humanoid
ev: 3 for 4 minions
stamina: "3"
immunities:
  - Poison 2
speed: 5
movement: Climb, swim
size: 1S
stability: 0
free_strike: 2
with_captain: +4 bonus to ranged distance
might: 0
agility: 2
reason: 1
intuition: 0
presence: 0
traits:
  - name: Toxiferous
    effects:
      - effect: Whenever an adjacent enemy grabs the dart or uses a melee ability
          against them, that enemy takes 1 poison damage.
abilities:
  - name: Poison Dart
    cost: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 8
    target: One creature per minion
    effects:
      - roll: Power Roll + 2
        t1: 2 poison damage
        t3: 5 poison damage
      - effect: The dart gains an edge on this ability against any target who has less
          than full Stamina.
```