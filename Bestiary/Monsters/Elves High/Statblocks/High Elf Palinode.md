---
agility: 0
ancestry:
- Fey
- High Elf
- Humanoid
ev: '6'
file_basename: High Elf Palinode
file_dpath: Monsters/Elves High/Statblocks
free_strike: 3
intuition: 2
item_id: high-elf-palinode
item_index: '111'
item_name: High Elf Palinode
level: 1
might: 0
presence: 1
reason: 0
roles:
- Platoon Support
scc:
- mcdm.monsters.v1:monster:high-elf-palinode
scdc:
- 1.1.1:2:111
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '30'
type: monster
---

```ds-statblock
name: High Elf Palinode
level: 1
roles:
  - Platoon Support
ancestry:
  - Fey
  - High Elf
  - Humanoid
ev: "6"
stamina: "30"
immunities:
  - Psychic 5
speed: 5
size: 1M
stability: 0
free_strike: 3
might: 0
agility: 0
reason: 0
intuition: 2
presence: 1
traits:
  - name: Otherworldly Grace
    effects:
      - effect: At the start of each of their turns, the palinode can choose one effect
          on them that can be ended by a saving throw. That effect instead ends
          at the end of their turn.
abilities:
  - name: Instill Regret
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 8
    target: One creature
    effects:
      - roll: Power Roll + 2
        t1: 5 psychic damage
        t2: 7 psychic damage; I < 1 weakened (save ends)
        t3: 9 psychic damage; I < 2 weakened (save ends)
      - effect: The potency increases by 1. If the target is weakened this way at the
          end of the encounter, they can't take a respite activity during their
          next respite.
        cost: 2 Malice
  - name: Recall
    icon: 🏹
    keywords:
      - Magic
      - Ranged
    type: Maneuver
    distance: Ranged 5
    target: Two allies
    effects:
      - effect: Each target can teleport to an unoccupied space adjacent to the
          palinode. The palinode and each target then gain 5 temporary Stamina.
        name: Effect
```