---
agility: 1
ancestry:
- Giant
- Troll
ev: 7 for four minions
file_basename: Troll Whelp
file_dpath: Monsters/Trolls/Statblocks
free_strike: 3
intuition: 0
item_id: troll-whelp
item_index: '410'
item_name: Troll Whelp
level: 5
might: 3
presence: 0
reason: -1
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster:troll-whelp
scdc:
- 1.1.1:2:410
size: 1L
source: mcdm.monsters.v1
speed: 6
stability: 3
stamina: '10'
type: monster
---

~~~ds-statblock
name: Troll Whelp
level: 5
roles:
  - Minion Brute
ancestry:
  - Giant
  - Troll
ev: 7 for four minions
stamina: "10"
weaknesses:
  - Acid 5
  - fire
speed: 6
size: 1L
stability: 3
free_strike: 3
with_captain: +2 damage bonus to strikes
might: 3
agility: 1
reason: -1
intuition: 0
presence: 0
traits:
  - name: Lingering Hunger
    effects:
      - effect: Whenever two or more whelps are simultaneously reduced to 0 Stamina by
          damage that isn't acid or fire damage, half of those whelps become
          troll limbjumbles with 4 Stamina.
abilities:
  - name: Jaws and Claws
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
      - roll: Power Roll + 3
        t1: 3 damage
        t2: 6 damage; slide 1
        t3: 7 damage; slide 2; M < 2 bleeding (save ends)
~~~