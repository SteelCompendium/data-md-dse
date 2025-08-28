---
agility: 3
ancestry:
- Goblin
- Hobgoblin
- Humanoid
- Infernal
ev: 6 for four minions
file_basename: Hobgoblin Lancer
file_dpath: Monsters/Hobgoblins/Statblocks
free_strike: 2
intuition: 2
item_id: hobgoblin-lancer
item_index: '182'
item_name: Hobgoblin Lancer
level: 4
might: 1
presence: 0
reason: 0
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster:hobgoblin-lancer
scdc:
- 1.1.1:2:182
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '8'
type: monster
---

~~~ds-statblock
name: Hobgoblin Lancer
level: 4
roles:
  - Minion Harrier
ancestry:
  - Goblin
  - Hobgoblin
  - Humanoid
  - Infernal
ev: 6 for four minions
stamina: "8"
immunities:
  - Fire 2
speed: 7
size: 1M
stability: 0
free_strike: 2
with_captain: +2 damage bonus to strikes
might: 1
agility: 3
reason: 0
intuition: 2
presence: 0
traits:
  - name: Infernal Ichor
    effects:
      - effect: When the lancer is reduced to 0 Stamina, they spray burning blood. Each
          creature adjacent to the lancer takes 2 fire damage.
abilities:
  - name: Grim Thrust
    icon: ⚔️
    cost: Signature Ability
    keywords:
      - Magic
      - Melee
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2 or ranged 5
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 3
        t1: 2 corruption damage
        t2: 4 corruption damage; push 1
        t3: 6 corruption damage; push 2
      - effect: The lancer deals an extra 2 damage if they have high ground against the
          target.
        name: Effect
~~~