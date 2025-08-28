---
agility: 2
ancestry:
- Angulotl
- Humanoid
ev: '3'
file_basename: Angulotl Needler
file_dpath: Monsters/Angulotls/Statblocks
free_strike: 2
intuition: 0
item_id: angulotl-needler
item_index: '244'
item_name: Angulotl Needler
level: 1
might: 0
presence: -1
reason: 1
roles:
- Horde Artillery
scc:
- mcdm.monsters.v1:monster:angulotl-needler
scdc:
- 1.1.1:2:244
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '10'
type: monster
---

```ds-statblock
name: Angulotl Needler
level: 1
roles:
  - Horde Artillery
ancestry:
  - Angulotl
  - Humanoid
ev: "3"
stamina: "10"
immunities:
  - Poison 2
speed: 5
movement: Climb, swim
size: 1S
stability: 0
free_strike: 2
might: 0
agility: 2
reason: 1
intuition: 0
presence: -1
traits:
  - name: Toxiferous
    effects:
      - effect: Whenever an adjacent enemy grabs the needler or uses a melee ability
          against them, that enemy takes 2 poison damage.
abilities:
  - name: Blowgun
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 15
    target: One creature
    effects:
      - roll: Power Roll + 2
        t1: 4 poison damage
        t2: 6 poison damage
        t3: 7 poison damage
      - effect: A target who has M < 2 is weakened (save ends). A target weakened this
          way takes 2 poison damage at the start of each of their turns.
        cost: 2 Malice
```