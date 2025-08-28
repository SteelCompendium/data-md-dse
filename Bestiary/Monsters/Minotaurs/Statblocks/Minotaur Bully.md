---
agility: 2
ancestry:
- Accursed
- Humanoid
- Minotaur
ev: 10 for four minions
file_basename: Minotaur Bully
file_dpath: Monsters/Minotaurs/Statblocks
free_strike: 4
intuition: 3
item_id: minotaur-bully
item_index: '176'
item_name: Minotaur Bully
level: 8
might: 4
presence: -1
reason: 0
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster:minotaur-bully
scdc:
- 1.1.1:2:176
size: '2'
source: mcdm.monsters.v1
speed: 6
stability: 2
stamina: '14'
type: monster
---

```ds-statblock
name: Minotaur Bully
level: 8
roles:
  - Minion Brute
ancestry:
  - Accursed
  - Humanoid
  - Minotaur
ev: 10 for four minions
stamina: "14"
speed: 6
size: "2"
stability: 2
free_strike: 4
with_captain: +3 damage bonus to strikes
might: 4
agility: 2
reason: 0
intuition: 3
presence: -1
traits:
  - name: Minotaur Sense
    effects:
      - effect: The bully can't obtain less than a tier 2 outcome when making tests to
          navigate, search, or seek.
abilities:
  - name: Javelin and Bellow
    icon: ⚔️
    cost: Signature Ability
    keywords:
      - Charge
      - Melee
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2 or ranged 5
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 4
        t1: 4 damage
        t2: 7 damage
        t3: 9 damage; I < 4 taunted (EoT) or frightened of all minotaurs (save ends)
```