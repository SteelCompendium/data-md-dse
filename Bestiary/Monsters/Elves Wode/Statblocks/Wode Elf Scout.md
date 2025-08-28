---
agility: 2
ancestry:
- Fey
- Humanoid
- Wode Elf
ev: 3 for four minions
file_basename: Wode Elf Scout
file_dpath: Monsters/Elves Wode/Statblocks
free_strike: 2
intuition: 0
item_id: wode-elf-scout
item_index: '224'
item_name: Wode Elf Scout
level: 1
might: 0
presence: 1
reason: 0
roles:
- Minion Ambusher
scc:
- mcdm.monsters.v1:monster:wode-elf-scout
scdc:
- 1.1.1:2:224
size: 1M
source: mcdm.monsters.v1
speed: 10
stability: 0
stamina: '4'
type: monster
---

~~~ds-statblock
name: Wode Elf Scout
level: 1
roles:
  - Minion Ambusher
ancestry:
  - Fey
  - Humanoid
  - Wode Elf
ev: 3 for four minions
stamina: "4"
speed: 10
size: 1M
stability: 0
free_strike: 2
with_captain: Gain an edge on strikes
might: 0
agility: 2
reason: 0
intuition: 0
presence: 1
traits:
  - name: Into the Green
    effects:
      - effect: The scout can attempt to hide at the end of each of their turns.
  - name: Masking Glamor
    effects:
      - effect: Abilities targeting the scout that would take a bane from cover or
          concealment have a double bane instead.
abilities:
  - name: Daggers
    icon: ⚔️
    cost: Signature Ability
    keywords:
      - Melee
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1 or ranged 5
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        t1: 2 damage
        t2: 4 damage
        t3: 5 damage
~~~