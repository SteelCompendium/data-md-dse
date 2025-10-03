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
item_index: '222'
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
- 1.1.1:2:222
size: 1M
source: mcdm.monsters.v1
speed: 10
stability: 0
stamina: '4'
type: monster
---

~~~ds-statblock
type: statblock
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
features:
  - type: feature
    feature_type: ability
    name: Daggers
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Melee
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1 or ranged 5
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 2 damage
        tier2: 4 damage
        tier3: 5 damage
  - type: feature
    feature_type: trait
    name: Into the Green
    icon: ⭐️
    effects:
      - effect: The scout can attempt to hide at the end of each of their turns.
  - type: feature
    feature_type: trait
    name: Masking Glamor
    icon: ⭐️
    effects:
      - effect: Abilities targeting the scout that would take a bane from cover or
          concealment have a double bane instead.
~~~