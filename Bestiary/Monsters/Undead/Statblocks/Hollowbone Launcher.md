---
agility: 3
ancestry:
- Undead
- Soulless
ev: 6 for four minions
file_basename: Hollowbone Launcher
file_dpath: Monsters/Undead/Statblocks
free_strike: 3
intuition: 0
item_id: hollowbone-launcher
item_index: '57'
item_name: Hollowbone Launcher
level: 4
might: -2
presence: 0
reason: 0
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster:hollowbone-launcher
scdc:
- 1.1.1:2:57
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '7'
type: monster
---

~~~ds-statblock
name: Hollowbone Launcher
level: 4
roles:
  - Minion Artillery
ancestry:
  - Undead
  - Soulless
ev: 6 for four minions
stamina: "7"
immunities:
  - Corruption 4
  - poison 4
speed: 5
size: 1M
stability: 0
free_strike: 3
with_captain: +5 bonus to ranged distance
might: -2
agility: 3
reason: 0
intuition: 0
presence: 0
traits:
  - name: Brittle Revenge
    effects:
      - effect: The hollowbone launcher explodes when they are reduced to 0 Stamina,
          dealing 2 damage to each adjacent creature
abilities:
  - name: Hollowbone Slug
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 10
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 3
        t1: 3 damage
        t2: 5 damage
        t3: 7 damage; M < 3 bleeding (save ends)
      - effect: Each creature adjacent to the target takes 2 damage.
        name: Effect
~~~