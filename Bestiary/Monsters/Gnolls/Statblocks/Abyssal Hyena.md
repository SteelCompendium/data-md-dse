---
agility: 1
ancestry:
- Abyssal
- Animal
- Gnoll
ev: 4 for four minions
file_basename: Abyssal Hyena
file_dpath: Monsters/Gnolls/Statblocks
free_strike: 3
intuition: 0
item_id: abyssal-hyena
item_index: '45'
item_name: Abyssal Hyena
level: 2
might: 2
presence: -2
reason: -3
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster:abyssal-hyena
scdc:
- 1.1.1:2:45
size: 1M
source: mcdm.monsters.v1
speed: 8
stability: 1
stamina: '7'
type: monster
---

```ds-statblock
name: Abyssal Hyena
level: 2
roles:
  - Minion Brute
ancestry:
  - Abyssal
  - Animal
  - Gnoll
ev: 4 for four minions
stamina: "7"
speed: 8
size: 1M
stability: 1
free_strike: 3
with_captain: +2 bonus to speed
might: 2
agility: 1
reason: -3
intuition: 0
presence: -2
traits:
  - name: Death Snap
    effects:
      - effect: When the abyssal hyena is reduced to 0 Stamina, they can make a melee
          free strike before dying.
abilities:
  - name: Snapjaw
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
        t1: 3 damage
        t2: 4 damage
        t3: 6 damage; grabbed
```