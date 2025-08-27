---
agility: -2
ancestry:
- Undead
- Soulless
ev: 3 for four minions
file_basename: Rotting Zombie
file_dpath: Monsters/Undead/Statblocks
free_strike: 2
intuition: -2
item_id: rotting-zombie
item_index: '76'
item_name: Rotting Zombie
level: 1
might: 2
presence: -3
reason: -5
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster:rotting-zombie
scdc:
- 1.1.1:2:76
size: 1M
source: mcdm.monsters.v1
speed: 4
stability: 0
stamina: '5'
type: monster
---

```ds-statblock
name: Rotting Zombie
level: 1
roles:
  - Minion Brute
ancestry:
  - Undead
  - Soulless
ev: 3 for four minions
stamina: "5"
immunities:
  - Corruption 1
  - poison 1
speed: 4
size: 1M
stability: 0
free_strike: 2
with_captain: +1 damage bonus to strikes
might: 2
agility: -2
reason: -5
intuition: -2
presence: -3
traits:
  - name: Death Grasp
    effects:
      - effect: When the rotting zombie is reduced to 0 Stamina, their space is
          difficult terrain. The first time any enemy who has M < 2 enters this
          space, they are slowed (save ends) and the effect end.
abilities:
  - name: Rotting Fist
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
      - roll: Power Roll + 2
        t1: 2 damage
        t2: 4 damage
        t3: 5 damage; M < 2 prone if size 1, or slowed (save ends) otherwise
```