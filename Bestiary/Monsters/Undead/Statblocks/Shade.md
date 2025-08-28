---
agility: 1
ancestry:
- Undead
ev: 3 for four minions
file_basename: Shade
file_dpath: Monsters/Undead/Statblocks
free_strike: 2
intuition: 0
item_id: shade
item_index: '65'
item_name: Shade
level: 1
might: -5
presence: 2
reason: 0
roles:
- Minion Ambusher
scc:
- mcdm.monsters.v1:monster:shade
scdc:
- 1.1.1:2:65
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '4'
type: monster
---

```ds-statblock
name: Shade
level: 1
roles:
  - Minion Ambusher
ancestry:
  - Undead
ev: 3 for four minions
stamina: "4"
immunities:
  - Corruption 1
  - poison 1
speed: 5
movement: Fly, hover
size: 1M
stability: 1
free_strike: 2
with_captain: +2 bonus to speed
might: -5
agility: 1
reason: 0
intuition: 0
presence: 2
traits:
  - name: Shadow Phasing
    effects:
      - effect: The shade can move through creatures and objects at their usual speed,
          but can't end their turn inside a creature or object. The first time
          in a round that the shade moves through a creature, that creature
          takes 1 corruption damage. The shade doesn't take damage from being
          force moved into objects.
abilities:
  - name: Life Drain
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
        t1: 2 corruption damage
        t2: 4 corruption damage
        t3: 5 corruption damage; the target must move up to their speed and can't end
          that movement closer to any shade
```