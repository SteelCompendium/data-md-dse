---
agility: -1
ancestry:
- Undead
- Soulless
ev: 6 for four minions
file_basename: Fleshflayed Shambler Zombie
file_dpath: Monsters/Undead/Statblocks
free_strike: 3
intuition: 0
item_id: fleshflayed-shambler-zombie
item_index: '81'
item_name: Fleshflayed Shambler Zombie
level: 4
might: 3
presence: 0
reason: 0
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster:fleshflayed-shambler-zombie
scdc:
- 1.1.1:2:81
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '9'
type: monster
---

```ds-statblock
name: Fleshflayed Shambler Zombie
level: 4
roles:
  - Minion Brute
ancestry:
  - Undead
  - Soulless
ev: 6 for four minions
stamina: "9"
immunities:
  - Corruption 4
  - poison 4
speed: 5
size: 1M
stability: 0
free_strike: 3
with_captain: +2 damage bonus to strikes
might: 3
agility: -1
reason: 0
intuition: 0
presence: 0
traits:
  - name: Fleshfused Spines
    effects:
      - effect: Any adjacent enemy who grabs the fleshflayed shambler or uses melee
          ability against them takes 2 damage.
abilities:
  - name: Bone Carvers
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 3
        t1: 3 damage
        t2: 5 damage
        t3: 7 damage
      - effect: If this ability gains an edge or has a double edge, the target is
          bleeding (save ends).
```