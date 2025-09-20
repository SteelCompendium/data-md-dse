---
agility: 2
ancestry:
- Fey
- High Elf
- Humanoid
ev: 3 for four minions
file_basename: High Elf Quiver
file_dpath: Monsters/Elves High/Statblocks
free_strike: 2
intuition: 0
item_id: high-elf-quiver
item_index: '108'
item_name: High Elf Quiver
level: 1
might: 0
presence: 0
reason: 1
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster:high-elf-quiver
scdc:
- 1.1.1:2:108
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '3'
type: monster
---

~~~ds-statblock
type: statblock
name: High Elf Quiver
level: 1
roles:
  - Minion Artillery
ancestry:
  - Fey
  - High Elf
  - Humanoid
ev: 3 for four minions
stamina: "3"
speed: 5
size: 1M
stability: 0
free_strike: 2
with_captain: +5 bonus to ranged distance
might: 0
agility: 2
reason: 1
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Heavy Arrow
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 10
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        tier1: 2 damage
        tier2: 4 damage
        tier3: 5 damage
      - name: Effect
        effect: Each ally adjacent to the target shifts up to 2 squares
  - type: feature
    feature_type: trait
    name: Otherworldly Grace
    icon: ⭐️
    effects:
      - effect: At the start of each of their turns, the quiver can choose one effect on
          them that can be ended by a saving throw. That effect instead ends at
          the end of their turn.
~~~