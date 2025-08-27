---
agility: 3
ancestry:
- Humanoid
- Rival
ev: '28'
file_basename: Rival Null
file_dpath: Monsters/Rivals/2nd Echelon/Statblocks
free_strike: 6
intuition: 3
item_id: rival-null
item_index: '14'
item_name: Rival Null
level: 5
might: 0
presence: 0
reason: 2
roles:
- Elite Harrier
scc:
- mcdm.monsters.v1:monster:rival-null
scdc:
- 1.1.1:2:14
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 3
stamina: '140'
type: monster
---

```ds-statblock
name: Rival Null
level: 5
roles:
  - Elite Harrier
ancestry:
  - Humanoid
  - Rival
ev: "28"
stamina: "140"
speed: 7
size: 1M
stability: 3
free_strike: 6
might: 0
agility: 3
reason: 2
intuition: 3
presence: 0
traits:
  - name: Inertial Shield
    effects:
      - effect: The first time each round that the null is targeted by a damage-dealing
          strike, they halve the damage.
  - name: Rivalry
    effects:
      - effect: At the start of an encounter, the null chooses one creature within their
          line of effect. Both the null and the creature can add a d3 roll to
          power rolls they make against each other.
abilities:
  - name: Agile Stride
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        t1: 9 damage; the null shifts up to 3 squares; A < 1 6 damage
        t2: 14 damage; the null shifts up to 4 squares; A < 2 11 damage
        t3: 17 damage; the null shifts up to 5 squares; A < 3 11 damage
  - name: Deaden
    icon: 🗡
    cost: 2 Malice
    keywords:
      - Melee
      - Psionic
      - Strike
      - Weapon
    type: Maneuver
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        t1: 9 damage; R < 1 dazed (EoT)
        t2: 14 damage; R < 2 dazed (save ends)
        t3: 17 damage; R < 3 dazed and restrained (save ends)
```