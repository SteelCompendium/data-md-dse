---
agility: 1
ancestry:
- Human
- Humanoid
ev: 4 for four minions
file_basename: Human Apprentice Mage
file_dpath: Monsters/Humans/Statblocks
free_strike: 2
intuition: 0
item_id: human-apprentice-mage
item_index: '164'
item_name: Human Apprentice Mage
level: 2
might: 0
presence: 2
reason: 0
roles:
- Minion Controller
scc:
- mcdm.monsters.v1:monster:human-apprentice-mage
scdc:
- 1.1.1:2:164
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '4'
type: monster
---

```ds-statblock
name: Human Apprentice Mage
level: 2
roles:
  - Minion Controller
ancestry:
  - Human
  - Humanoid
ev: 4 for four minions
stamina: "4"
immunities:
  - Corruption 2
  - psychic 2
speed: 5
size: 1M
stability: 0
free_strike: 2
with_captain: +5 bonus to ranged distance
might: 0
agility: 1
reason: 0
intuition: 0
presence: 2
traits:
  - name: Supernatural Insight
    effects:
      - effect: The apprentice mage ignores concealment if it's granted by a
          supernatural effect.
abilities:
  - name: Lightning Strike
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 10
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        t1: 2 lightning damage
        t2: 3 lightning damage
        t3: 5 lightning damage
      - effect: If the apprentice mage doesn't use a maneuver or a move action this
          turn, the target is also slowed (EoT).
        name: Effect
```