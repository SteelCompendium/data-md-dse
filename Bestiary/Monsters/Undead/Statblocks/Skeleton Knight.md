---
agility: 5
ancestry:
- Undead
- Soulless
ev: 12 for four minions
file_basename: Skeleton Knight
file_dpath: Monsters/Undead/Statblocks
free_strike: 4
intuition: 4
item_id: skeleton-knight
item_index: '60'
item_name: Skeleton Knight
level: 10
might: 3
presence: -2
reason: -2
roles:
- Minion Defender
scc:
- mcdm.monsters.v1:monster:skeleton-knight
scdc:
- 1.1.1:2:60
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '17'
type: monster
---

~~~ds-statblock
name: Skeleton Knight
level: 10
roles:
  - Minion Defender
ancestry:
  - Undead
  - Soulless
ev: 12 for four minions
stamina: "17"
immunities:
  - Corruption 10
  - poison 10
speed: 5
size: 1L
stability: 2
free_strike: 4
with_captain: Gain an edge on strikes
might: 3
agility: 5
reason: -2
intuition: 4
presence: -2
traits:
  - name: Bitter Bones
    effects:
      - effect: If the knight is reduced to 0 Stamina, their bones collapse to fill
          their space with an impassable barrier. Any enemy who comes adjacent
          to the barrier for the first time in a round or starts their turn
          there takes 5 damage.
  - name: More Swings
    effects:
      - effect: Whenever the knight makes a free strike, they can make two free strikes
          instead.
abilities:
  - name: Four Swords Swing
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 5
        t1: 4 damage
        t2: 7 damage
        t3: 9 damage; the target can't shift (EoT
~~~