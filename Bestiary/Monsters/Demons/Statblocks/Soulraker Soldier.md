---
agility: 2
ancestry:
- Abyssal
- Demon
- Soulraker
ev: 9 for four minions
file_basename: Soulraker Soldier
file_dpath: Monsters/Demons/Statblocks
free_strike: 4
intuition: -1
item_id: soulraker-soldier
item_index: '273'
item_name: Soulraker Soldier
level: 7
might: 4
presence: -1
reason: -1
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster:soulraker-soldier
scdc:
- 1.1.1:2:273
size: '2'
source: mcdm.monsters.v1
speed: 6
stability: 2
stamina: '13'
type: monster
---

```ds-statblock
name: Soulraker Soldier
level: 7
roles:
  - Minion Brute
ancestry:
  - Abyssal
  - Demon
  - Soulraker
ev: 9 for four minions
stamina: "13"
weaknesses:
  - Holy 5
speed: 6
size: "2"
stability: 2
free_strike: 4
with_captain: Gain an edge on strikes
might: 4
agility: 2
reason: -1
intuition: -1
presence: -1
traits:
  - name: Abyssal Buzzing
    effects:
      - effect: Any enemy who starts their turn with two or more soulraker minions
          adjacent to them takes 3 sonic damage.
abilities:
  - name: Chitin Bash
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
      - roll: Power Roll + 4
        t1: 4 damage; push 2
        t2: 7 damage; push 2
        t3: 8 damage; push 4
```