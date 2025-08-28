---
agility: 2
ancestry:
- Humanoid
- Time Raider
ev: 5 for four minions
file_basename: Time Raider Archon
file_dpath: Monsters/Time Raiders/Statblocks
free_strike: 2
intuition: 1
item_id: time-raider-archon
item_index: '143'
item_name: Time Raider Archon
level: 3
might: 2
presence: -1
reason: 2
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster:time-raider-archon
scdc:
- 1.1.1:2:143
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '7'
type: monster
---

~~~ds-statblock
name: Time Raider Archon
level: 3
roles:
  - Minion Harrier
ancestry:
  - Humanoid
  - Time Raider
ev: 5 for four minions
stamina: "7"
immunities:
  - Psychic 3
speed: 7
size: 1M
stability: 0
free_strike: 2
with_captain: +1 damage bonus to strikes
might: 2
agility: 2
reason: 2
intuition: 1
presence: -1
traits:
  - name: Foresight
    effects:
      - effect: The archon doesn't take a bane on strikes against creatures with
          concealment.
abilities:
  - name: Brutal Flail
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Psionic
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        t1: 2 damage
        t2: 4 damage
        t3: 5 damage; one ally can make a free strike against the target
~~~