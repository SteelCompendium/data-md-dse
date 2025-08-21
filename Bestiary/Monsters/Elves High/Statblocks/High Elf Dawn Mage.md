---
agility: 0
ancestry:
- Fey
- High Elf
- Humanoid
ev: 3 for four minions
file_basename: High Elf Dawn Mage
file_dpath: Monsters/Elves High/Statblocks
free_strike: 1
intuition: -1
item_id: high-elf-dawn-mage
item_index: '112'
item_name: High Elf Dawn Mage
level: 1
might: 0
presence: 1
reason: 2
roles:
- Minion Controller
scc:
- mcdm.monsters.v1:monster:high-elf-dawn-mage
scdc:
- 1.1.1:2:112
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '3'
type: monster
---

```ds-statblock
name: High Elf Dawn Mage
level: 1
roles:
  - Minion Controller
ancestry:
  - Fey
  - High Elf
  - Humanoid
ev: 3 for four minions
stamina: "3"
speed: 5
size: 1M
stability: 0
free_strike: 1
with_captain: +5 bonus to ranged distance
might: 0
agility: 0
reason: 2
intuition: -1
presence: 1
traits:
  - name: Otherworldly Grace
    effects:
      - effect: At the start of each of their turns, the dawn mage can choose one effect
          on them that can be ended by a saving throw. That effect instead ends
          at the end of their turn.
abilities:
  - name: Bright Bolt
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 5
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        t1: 1 holy damage
        t2: 2 holy damage
        t3: 3 holy damage
      - effect: Until the start of the dawn mage's next turn, the target can't hide.
        name: Effect
```