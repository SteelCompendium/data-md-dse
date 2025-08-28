---
agility: -1
ancestry:
- Giant
- Hill Giant
ev: 9 for four minions
file_basename: Hill Giant Mosstooth
file_dpath: Monsters/Giants/Statblocks
free_strike: 4
intuition: -1
item_id: hill-giant-mosstooth
item_index: '197'
item_name: Hill Giant Mosstooth
level: 7
might: 4
presence: -1
reason: -1
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster:hill-giant-mosstooth
scdc:
- 1.1.1:2:197
size: '4'
source: mcdm.monsters.v1
speed: 6
stability: 5
stamina: '13'
type: monster
---

~~~ds-statblock
name: Hill Giant Mosstooth
level: 7
roles:
  - Minion Brute
ancestry:
  - Giant
  - Hill Giant
ev: 9 for four minions
stamina: "13"
immunities:
  - Damage 3
speed: 6
movement: Climb
size: "4"
stability: 5
free_strike: 4
with_captain: +3 damage bonus to strikes
might: 4
agility: -1
reason: -1
intuition: -1
presence: -1
traits:
  - name: Distracted
    effects:
      - effect: Whenever the mosstooth targets a creature or object with an ability, any
          enemy within distance of the ability can use a free triggered action
          to distract the mosstooth. The mosstooth targets that enemy instead.
abilities:
  - name: Swing
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 3
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 4
        t1: 4 damage
        t2: 7 damage
        t3: 8 damage; grabbed
      - effect: The mosstooth can use a creature or object they have grabbed as a weapon
          for this ability, dealing an extra 5 damage to that creature or object
          and the target. They then end the grab and leave the creature or
          object prone in an unoccupied space adjacent to the target.
        name: Effect
~~~