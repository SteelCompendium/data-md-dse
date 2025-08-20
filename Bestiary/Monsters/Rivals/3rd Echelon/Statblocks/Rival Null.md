---
agility: 4
ancestry:
- Humanoid
- Rival
ev: '40'
file_basename: Rival Null
file_dpath: Monsters/Rivals/3rd Echelon/Statblocks
free_strike: 8
intuition: 4
item_id: rival-null
item_index: '21'
item_name: Rival Null
level: 8
might: 2
presence: 0
reason: 3
roles:
- Elite Harrier
scc:
- mcdm.monsters.v1:monster:rival-null
scdc:
- 1.1.1:2:21
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 3
stamina: '200'
type: monster
---

```ds-statblock
name: Rival Null
level: 8
roles:
  - Elite Harrier
ancestry:
  - Humanoid
  - Rival
ev: "40"
stamina: "200"
speed: 7
size: 1M
stability: 3
free_strike: 8
might: 2
agility: 4
reason: 3
intuition: 4
presence: 0
traits:
  - name: Force Dampener
    effects:
      - effect: The first time each round that the null is targeted by a strike, it
          takes a bane and the null halves any damage from it.
  - name: Rivalry
    effects:
      - effect: At the start of an encounter, the null chooses one creature within their
          line of effect. Both the null and the creature can add a d3 roll to
          power rolls they make against each other.
abilities:
  - name: Inertial Flow
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        t1: 12 damage; the null shifts up to 3 squares; A < 2 8 damage
        t2: 17 damage; the null shifts up to 4 squares; A < 3 13 damage
        t3: 21 damage; the null shifts up to 5 squares; A < 4 17 damage
  - name: Stun
    cost: 3 Malice
    keywords:
      - Melee
      - Psionic
      - Strike
      - Weapon
    type: Maneuver
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        t1: 12 damage; R < 2 dazed (save ends)
        t2: 17 damage; R < 3 dazed (save ends)
        t3: 21 damage; R < 4 dazed and restrained (save ends)
```