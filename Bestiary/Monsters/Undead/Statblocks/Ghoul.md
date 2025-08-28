---
agility: 2
ancestry:
- Undead
ev: '3'
file_basename: Ghoul
file_dpath: Monsters/Undead/Statblocks
free_strike: 1
intuition: 0
item_id: ghoul
item_index: '77'
item_name: Ghoul
level: 1
might: 0
presence: -1
reason: -2
roles:
- Horde Harrier
scc:
- mcdm.monsters.v1:monster:ghoul
scdc:
- 1.1.1:2:77
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '15'
type: monster
---

```ds-statblock
name: Ghoul
level: 1
roles:
  - Horde Harrier
ancestry:
  - Undead
ev: "3"
stamina: "15"
immunities:
  - Corruption 1
  - poison 1
speed: 7
size: 1M
stability: 0
free_strike: 1
might: 0
agility: 2
reason: -2
intuition: 0
presence: -1
traits:
  - name: Arise
    effects:
      - effect: The first time the ghoul is reduced to 0 Stamina by damage that isn't
          fire damage or holy damage and their body isn't destroyed, they
          instead have 1 Stamina and fall prone.
  - name: Hunger
    effects:
      - effect: When the ghoul uses the Charge main action, they gain a +2 bonus to
          speed until the end of their turn.
abilities:
  - name: Razor Claws
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 3 damage
        t2: 4 damage
        t3: 5 damage; M < 2 bleeding (save ends)
  - name: Leap
    icon: 👤
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The ghoul jumps up to 3 squares. If they land on a size 1 enemy, that
          enemy is knocked prone and the ghoul can make a free strike against
          them.
        name: Effect
```