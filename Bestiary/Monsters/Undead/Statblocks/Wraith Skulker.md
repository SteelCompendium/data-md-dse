---
agility: 3
ancestry:
- Undead
ev: 12 for four minions
file_basename: Wraith Skulker
file_dpath: Monsters/Undead/Statblocks
free_strike: 4
intuition: 1
item_id: wraith-skulker
item_index: '86'
item_name: Wraith Skulker
level: 10
might: -2
presence: 5
reason: 1
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster:wraith-skulker
scdc:
- 1.1.1:2:86
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 1
stamina: '15'
type: monster
---

```ds-statblock
name: Wraith Skulker
level: 10
roles:
  - Minion Harrier
ancestry:
  - Undead
ev: 12 for four minions
stamina: "15"
immunities:
  - Corruption 10
  - poison 10
speed: 7
movement: Fly, hover
size: 1M
stability: 1
free_strike: 4
with_captain: +3 bonus to speed
might: -2
agility: 3
reason: 1
intuition: 1
presence: 5
traits:
  - name: Corruptive Phasing
    effects:
      - effect: The wraith can move through creatures and objects at their usual speed,
          but can't end their turn inside a creature or object. The first time
          in a round that the wraith moves through a creature, that creature
          takes 5 corruption damage. The wraith doesn't take damage from being
          force moved into objects.
abilities:
  - name: Draining Rake
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 5
        t1: 4 cold damage; the wraith can shift 1 squar
        t2: 7 cold damage; the wraith shifts up to 2 square
        t3: 9 cold damage; P < 5 slowed (save ends); the wraith shifts up to 3 squares
      - effect: The wraith turns invisible until the start of their next turn.
        name: Effect
```