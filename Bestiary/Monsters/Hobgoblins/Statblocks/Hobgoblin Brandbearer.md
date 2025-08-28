---
agility: 1
ancestry:
- Goblin
- Hobgoblin
- Humanoid
- Infernal
ev: 6 for four minions
file_basename: Hobgoblin Brandbearer
file_dpath: Monsters/Hobgoblins/Statblocks
free_strike: 2
intuition: 0
item_id: hobgoblin-brandbearer
item_index: '187'
item_name: Hobgoblin Brandbearer
level: 4
might: 0
presence: 3
reason: 2
roles:
- Minion Hexer
scc:
- mcdm.monsters.v1:monster:hobgoblin-brandbearer
scdc:
- 1.1.1:2:187
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '7'
type: monster
---

~~~ds-statblock
name: Hobgoblin Brandbearer
level: 4
roles:
  - Minion Hexer
ancestry:
  - Goblin
  - Hobgoblin
  - Humanoid
  - Infernal
ev: 6 for four minions
stamina: "7"
immunities:
  - Fire 2
speed: 5
size: 1M
stability: 0
free_strike: 2
with_captain: Gain an edge on strikes
might: 0
agility: 1
reason: 2
intuition: 0
presence: 3
traits:
  - name: Open Furnace
    effects:
      - effect: Whenever an enemy takes fire damage, they take 1 extra fire damage for
          each brandbearer adjacent to them.
  - name: Infernal Ichor
    effects:
      - effect: When the brandbearer is reduced to 0 Stamina, they spray burning blood.
          Each creature adjacent to the brandbearer takes 2 fire damage.
abilities:
  - name: Searing Grasp
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Magic
      - Melee
      - Strike
    type: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 3
        t1: 2 fire damage
        t2: 4 fire damage; M < 2 fire weakness 5 (save ends)
        t3: 6 fire damage; M < 3 fire weakness 5 (save ends)
~~~