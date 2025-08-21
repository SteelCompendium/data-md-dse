---
agility: 2
ancestry:
- Human
- Humanoid
ev: 3 for four minions
file_basename: Human Rogue
file_dpath: Monsters/Humans/Statblocks
free_strike: 2
intuition: 0
item_id: human-rogue
item_index: '157'
item_name: Human Rogue
level: 1
might: 0
presence: 1
reason: 0
roles:
- Minion Ambusher
scc:
- mcdm.monsters.v1:monster:human-rogue
scdc:
- 1.1.1:2:157
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '4'
type: monster
---

```ds-statblock
name: Human Rogue
level: 1
roles:
  - Minion Ambusher
ancestry:
  - Human
  - Humanoid
ev: 3 for four minions
stamina: "4"
immunities:
  - Corruption 1
  - psychic 1
speed: 7
size: 1M
stability: 0
free_strike: 2
with_captain: Gain an edge on strikes
might: 0
agility: 2
reason: 0
intuition: 0
presence: 1
traits:
  - name: Supernatural Insight
    effects:
      - effect: The rogue ignores concealment if it's granted by a supernatural effect.
abilities:
  - name: Concealed Dagger
    cost: Signature Ability
    keywords:
      - Melee
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1 or Ranged 5
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        t1: 1 damage
        t2: 2 damage
        t3: 3 damage
      - effect: If the rogue is disguised or hidden when they use this ability, it deals
          an extra 3 damage.
        name: Effect
```