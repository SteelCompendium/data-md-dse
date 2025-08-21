---
agility: 3
ancestry:
- Horror
- Voiceless Talker
ev: 8 for four minions
file_basename: Mindkiller Whelp
file_dpath: Monsters/Voiceless Talkers/Statblocks
free_strike: 3
intuition: 1
item_id: mindkiller-whelp
item_index: '338'
item_name: Mindkiller Whelp
level: 6
might: -1
presence: 0
reason: 1
roles:
- Minion Hexer
scc:
- mcdm.monsters.v1:monster:mindkiller-whelp
scdc:
- 1.1.1:2:338
size: 1S
source: mcdm.monsters.v1
speed: 4
stability: 0
stamina: '9'
type: monster
---

```ds-statblock
name: Mindkiller Whelp
level: 6
roles:
  - Minion Hexer
ancestry:
  - Horror
  - Voiceless Talker
ev: 8 for four minions
stamina: "9"
immunities:
  - Psychic 6
speed: 4
movement: Fly, hover
size: 1S
stability: 0
free_strike: 3
with_captain: +2 damage bonus to strikes
might: -1
agility: 3
reason: 1
intuition: 1
presence: 0
traits:
  - name: Psionic Conductor
    effects:
      - effect: Whenever a non-minion voiceless talker within 5 squares of the whelp
          uses a psionic ability, they can do so as if they were in the whelp's
          space.
abilities:
  - name: Eager Claws
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
        t2: 5 damage; the target takes a bane on their next strike
        t3: 7 damage; the target takes a bane on their next strike
  - name: Feast
    keywords:
      - Psionic
    type: Triggered action
    distance: Self
    target: Self
    trigger: The whelp reduces a non-minion creature to 0 Stamina.
    effects:
      - effect: The whelp transforms into a mindkiller whose Stamina equals their
          squad's Stamina pool before transforming. The Stamina pool then loses
          the whelp's Stamina.
        name: Effect
```