---
agility: 2
ancestry:
- Humanoid
- Rival
ev: '16'
file_basename: Rival Null
file_dpath: Monsters/Rivals/1st Echelon/Statblocks
free_strike: 5
intuition: 2
item_id: rival-null
item_index: '07'
item_name: Rival Null
level: 2
might: 0
presence: 0
reason: 1
roles:
- Elite Harrier
scc:
- mcdm.monsters.v1:monster:rival-null
scdc:
- 1.1.1:2:07
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 3
stamina: '80'
type: monster
---

```ds-statblock
name: Rival Null
level: 2
roles:
  - Elite Harrier
ancestry:
  - Humanoid
  - Rival
ev: "16"
stamina: "80"
speed: 7
size: 1M
stability: 3
free_strike: 5
might: 0
agility: 2
reason: 1
intuition: 2
presence: 0
traits:
  - name: Inertial Shield
    effects:
      - effect: The first time each round that the null is targeted by a da- age-dealing
          strike, they halve the damage.
  - name: Rivalry
    effects:
      - effect: At the start of an encounter, the null chooses one creature within their
          line of effect. Both the null and the creature can add a d3 roll to
          power rolls they make against each other.
abilities:
  - name: Nimble Step
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        t1: 7 damage; the null shifts up to 2 square
        t2: 10 damage; the null shifts up to 3 squares
        t3: 13 damage; the null shifts up to 4 squares
  - name: Numb
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
      - roll: Power Roll + 2
        t1: 7 damage; R < 0 slowed (EoT)
        t2: 10 damage; R < 1 slowed (EoT)
        t3: 13 damage; R < 2 dazed and slowed (EoT)
```