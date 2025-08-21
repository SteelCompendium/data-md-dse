---
agility: 2
ancestry:
- Humanoid
- Soulless
- War Dog
ev: 12 for four minions
file_basename: War Dog Socialite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 4
intuition: 3
item_id: war-dog-socialite
item_index: '367'
item_name: War Dog Socialite
level: 10
might: 2
presence: 5
reason: 4
roles:
- Minion Hexer
scc:
- mcdm.monsters.v1:monster:war-dog-socialite
scdc:
- 1.1.1:2:367
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '14'
type: monster
---

```ds-statblock
name: War Dog Socialite
level: 10
roles:
  - Minion Hexer
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: 12 for four minions
stamina: "14"
immunities:
  - Psychic 10
speed: 5
size: 1M
stability: 0
free_strike: 4
with_captain: Gain an edge on strikes
might: 2
agility: 2
reason: 4
intuition: 3
presence: 5
traits:
  - name: Loyalty Collar
    effects:
      - effect: When the socialite is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 3d6 damage to each adjacent enemy and object.
abilities:
  - name: Call to Self-Sabotage
    cost: Signature Ability
    keywords:
      - Psionic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 5
    target: One creature per minion
    effects:
      - roll: Power Roll + 5
        t1: The target makes a free strike (tier 1 result) against themself
        t2: The target makes a free strike (tier 2 result) against themself
        t3: The target makes a free strike (tier 3 result) against themself
      - effect: The target takes an extra 5 damage for each surge they have.
        name: Effect
```