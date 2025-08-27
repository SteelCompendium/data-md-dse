---
agility: 3
ancestry:
- Abyssal
- Demon
ev: 12 for four minions
file_basename: Optacus
file_dpath: Monsters/Demons/Statblocks
free_strike: 5
intuition: 5
item_id: optacus
item_index: '282'
item_name: Optacus
level: 10
might: 1
presence: 1
reason: 1
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster:optacus
scdc:
- 1.1.1:2:282
size: 1S
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '14'
type: monster
---

```ds-statblock
name: Optacus
level: 10
roles:
  - Minion Artillery
ancestry:
  - Abyssal
  - Demon
ev: 12 for four minions
stamina: "14"
weaknesses:
  - Holy 5
speed: 6
movement: Climb
size: 1S
stability: 0
free_strike: 5
with_captain: +4 bonus to speed
might: 1
agility: 3
reason: 1
intuition: 5
presence: 1
traits: []
abilities:
  - name: Optical Flare
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 20
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 5
        t1: 5 fire damage
        t2: 8 fire damage
        t3: 10 fire damage; this damage ignores immunity
      - effect: This ability ignores concealment. A winded target takes an extra 5
          damage.
        name: Effect
```