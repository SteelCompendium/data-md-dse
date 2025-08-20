---
agility: 1
ancestry:
- Human
- Humanoid
ev: 3 for four minions
file_basename: Human Death Acolyte
file_dpath: Monsters/Humans/Statblocks
free_strike: 1
intuition: 0
item_id: human-death-acolyte
item_index: '161'
item_name: Human Death Acolyte
level: 1
might: 0
presence: 2
reason: 0
roles:
- Minion Hexer
scc:
- mcdm.monsters.v1:monster:human-death-acolyte
scdc:
- 1.1.1:2:161
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '3'
type: monster
---

```ds-statblock
name: Human Death Acolyte
level: 1
roles:
  - Minion Hexer
ancestry:
  - Human
  - Humanoid
ev: 3 for four minions
stamina: "3"
immunities:
  - Corruption 1
  - psychic 1
speed: 5
size: 1M
stability: 0
free_strike: 1
with_captain: +5 bonus to ranged distance
might: 0
agility: 1
reason: 0
intuition: 0
presence: 2
traits:
  - name: Supernatural Insight
    effects:
      - effect: The death acolyte ignores concealment if it's granted by a supernatural
          effect.
abilities:
  - name: Necrotic Bolt
    cost: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 10
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        t1: 1 corruption damage
        t2: 2 corruption damage
        t3: 3 corruption damage
      - effect: One creature within 5 squares regains 1 Stamina.
```