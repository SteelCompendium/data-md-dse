---
agility: 3
ancestry:
- Bugbear
- Fey
- Goblin
- Humanoid
ev: 10 for four minions
file_basename: Bugbear Knightmare
file_dpath: Monsters/Bugbears/Statblocks
free_strike: 3
intuition: 1
item_id: bugbear-knightmare
item_index: '293'
item_name: Bugbear Knightmare
level: 8
might: 4
presence: 4
reason: 1
roles:
- Minion Hexer
scc:
- mcdm.monsters.v1:monster:bugbear-knightmare
scdc:
- 1.1.1:2:293
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '12'
type: monster
---

~~~ds-statblock
name: Bugbear Knightmare
level: 8
roles:
  - Minion Hexer
ancestry:
  - Bugbear
  - Fey
  - Goblin
  - Humanoid
ev: 10 for four minions
stamina: "12"
speed: 5
size: 1L
stability: 2
free_strike: 3
with_captain: Gain an edge on strikes
might: 4
agility: 3
reason: 1
intuition: 1
presence: 4
traits:
  - name: Bu'gathic Inspiration
    effects:
      - effect: Any ally has a +1 bonus to power rolls, saving throws, or damage rolled
          as a d6 or a d3 for each knightmare adjacent to them.
  - name: Magic Terror
    effects:
      - effect: Each enemy has a −1 penalty to power rolls, saving throws, or damage
          rolled as a d6 or a d3 for each knightmare adjacent to them.
abilities:
  - name: Corrosive Blade
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Magic
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 4
        t1: 3 corruption damage
        t2: 6 corruption damage; P < 3 bleeding (save ends)
        t3: 8 corruption damage; grabbed; P < 4 bleeding (save ends)
      - effect: A target grabbed this way or already grabbed by the knightmare can be
          vertical pushed up to 5 squares.
        name: Effect
~~~