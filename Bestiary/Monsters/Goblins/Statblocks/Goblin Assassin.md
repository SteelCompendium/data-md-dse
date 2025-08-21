---
agility: 2
ancestry:
- Goblin
- Humanoid
ev: '3'
file_basename: Goblin Assassin
file_dpath: Monsters/Goblins/Statblocks
free_strike: 2
intuition: 0
item_id: goblin-assassin
item_index: '307'
item_name: Goblin Assassin
level: 1
might: -2
presence: -2
reason: 0
roles:
- Horde Ambusher
scc:
- mcdm.monsters.v1:monster:goblin-assassin
scdc:
- 1.1.1:2:307
size: 1S
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '15'
type: monster
---

```ds-statblock
name: Goblin Assassin
level: 1
roles:
  - Horde Ambusher
ancestry:
  - Goblin
  - Humanoid
ev: "3"
stamina: "15"
speed: 6
movement: Climb
size: 1S
stability: 0
free_strike: 2
might: -2
agility: 2
reason: 0
intuition: 0
presence: -2
traits:
  - name: Crafty
    effects:
      - effect: The assassin doesn't provoke opportunity attacks by moving.
  - name: Slip Away
    effects:
      - effect: The assassin can attempt to hide even while observed
abilities:
  - name: Sword Stab
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 4 damage
        t2: 6 damage
        t3: 7 damage
      - effect: If this ability gains an edge or has a double edge, it deals an extra 2
          damage.
        name: Effect
  - name: Shadow Chains
    cost: 3 Malice
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 10
    target: Three creatures
    effects:
      - roll: Power Roll + 2
        t1: 2 corruption damage; A < 0 restrained (save ends)
        t2: 4 corruption damage; A < 1 restrained (save ends)
        t3: 5 corruption damage; A < 2 restrained (save ends)
```