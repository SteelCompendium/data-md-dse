---
agility: 2
ancestry:
- Angulotl
- Humanoid
ev: 3 for 4 minions
file_basename: Angulotl Cleaver
file_dpath: Monsters/Angulotls/Statblocks
free_strike: 2
intuition: 1
item_id: angulotl-cleaver
item_index: '240'
item_name: Angulotl Cleaver
level: 1
might: 0
presence: 0
reason: 0
roles:
- Minion Ambusher
scc:
- mcdm.monsters.v1:monster:angulotl-cleaver
scdc:
- 1.1.1:2:240
size: 1S
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '4'
type: monster
---

```ds-statblock
name: Angulotl Cleaver
level: 1
roles:
  - Minion Ambusher
ancestry:
  - Angulotl
  - Humanoid
ev: 3 for 4 minions
stamina: "4"
immunities:
  - Poison 2
speed: 6
movement: Climb, swim
size: 1S
stability: 0
free_strike: 2
with_captain: +1 damage bonus to strikes
might: 0
agility: 2
reason: 0
intuition: 1
presence: 0
traits:
  - name: Toxiferous
    effects:
      - effect: Whenever an adjacent enemy grabs the cleaver or uses a melee ability
          against them, that enemy takes 1 poison damage.
abilities:
  - name: Hop and Chop
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        t1: 2 damage
        t2: 4 damage
        t3: 5 damage
      - effect: The cleaver jumps up to 4 squares before or after making this strike.
        name: Effect
```