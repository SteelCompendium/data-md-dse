---
agility: 3
ancestry:
- Bugbear
- Fey
- Goblin
- Humanoid
ev: 7 for four minions
file_basename: Bugbear Snare
file_dpath: Monsters/Bugbears/Statblocks
free_strike: 3
intuition: 0
item_id: bugbear-snare
item_index: '294'
item_name: Bugbear Snare
level: 5
might: 2
presence: 1
reason: 0
roles:
- Minion Ambusher
scc:
- mcdm.monsters.v1:monster:bugbear-snare
scdc:
- 1.1.1:2:294
size: 1L
source: mcdm.monsters.v1
speed: 6
stability: 2
stamina: '9'
type: monster
---

~~~ds-statblock
name: Bugbear Snare
level: 5
roles:
  - Minion Ambusher
ancestry:
  - Bugbear
  - Fey
  - Goblin
  - Humanoid
ev: 7 for four minions
stamina: "9"
speed: 6
size: 1L
stability: 2
free_strike: 3
with_captain: +3 bonus to speed
might: 2
agility: 3
reason: 0
intuition: 0
presence: 1
traits: []
abilities:
  - name: Cut 'Em Low!
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 3
        t1: 3 damage
        t2: 6 damage
        t3: 7 damage; A < 3 slowed (save ends)
      - effect: If the snare started their turn hidden from the target, the target is
          automatically grabbed. A target grabbed this way or already grabbed by
          the snare can be vertical pushed up to 4 squares.
        name: Effect
~~~