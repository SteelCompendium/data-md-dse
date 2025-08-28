---
agility: 1
ancestry:
- Humanoid
- Orc
ev: 3 for four minion
file_basename: Orc Bloodspark
file_dpath: Monsters/Orcs/Statblocks
free_strike: 2
intuition: 0
item_id: orc-bloodspark
item_index: '136'
item_name: Orc Bloodspark
level: 1
might: 0
presence: 2
reason: 0
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster:orc-bloodspark
scdc:
- 1.1.1:2:136
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '3'
type: monster
---

```ds-statblock
name: Orc Bloodspark
level: 1
roles:
  - Minion Artillery
ancestry:
  - Humanoid
  - Orc
ev: 3 for four minion
stamina: "3"
speed: 6
size: 1M
stability: 0
free_strike: 2
with_captain: +2 bonus to forced movement distance
might: 0
agility: 1
reason: 0
intuition: 0
presence: 2
traits:
  - name: Bloodfire Bur
    effects:
      - effect: If the bloodspark is reduced to 0 Stamina, they can make a free strike
          before dying.
abilities:
  - name: Explosive Mote
    icon: 🏹
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
        t1: 2 damage; push 1, or the bloodspark can shift 1 square away from the target
        t2: 4 damage; push 2, or the bloodspark shifts up to 2 squares away from the
          target
        t3: 5 damage; push 4, or the bloodspark shifts up to 4 squares away from the
          target
```