---
agility: 2
ancestry:
- Undead
ev: 6 for four minions
file_basename: Ghoul Craver
file_dpath: Monsters/Undead/Statblocks
free_strike: 2
intuition: 0
item_id: ghoul-craver
item_index: '70'
item_name: Ghoul Craver
level: 4
might: 3
presence: 0
reason: 0
roles:
- Minion Harrier
scc:
- mcdm.monsters.v1:monster:ghoul-craver
scdc:
- 1.1.1:2:70
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '8'
type: monster
---

~~~ds-statblock
type: statblock
name: Ghoul Craver
level: 4
roles:
  - Minion Harrier
ancestry:
  - Undead
ev: 6 for four minions
stamina: "8"
immunities:
  - Corruption 4
  - poison 4
speed: 7
movement: Climb
size: 1M
stability: 0
free_strike: 2
with_captain: +2 damage bonus to strikes
might: 3
agility: 2
reason: 0
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Taste
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 3
        tier1: 2 damage
        tier2: 4 damage
        tier3: 6 damage
      - name: Effect
        effect: This ability has a double edge against a bleeding target.
  - type: feature
    feature_type: trait
    name: Ever So Hungry
    icon: ⭐️
    effects:
      - effect: Any enemy adjacent to three or more ghoul cravers can't shift
  - type: feature
    feature_type: trait
    name: Hunger
    icon: ⭐️
    effects:
      - effect: When the ghoul craver uses the Charge main action, they gain a +2 bonus
          to speed until the end of their turn.
~~~