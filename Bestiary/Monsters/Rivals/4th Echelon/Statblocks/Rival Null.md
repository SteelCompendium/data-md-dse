---
agility: 5
ancestry:
- Humanoid
- Rival
ev: '48'
file_basename: Rival Null
file_dpath: Monsters/Rivals/4th Echelon/Statblocks
free_strike: 10
intuition: 5
item_id: rival-null
item_index: '28'
item_name: Rival Null
level: 10
might: 3
presence: 0
reason: 4
roles:
- Elite Harrier
scc:
- mcdm.monsters.v1:monster:rival-null
scdc:
- 1.1.1:2:28
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 3
stamina: '240'
type: monster
---

```ds-statblock
name: Rival Null
level: 10
roles:
  - Elite Harrier
ancestry:
  - Humanoid
  - Rival
ev: "48"
stamina: "240"
speed: 7
size: 1M
stability: 3
free_strike: 10
might: 3
agility: 5
reason: 4
intuition: 5
presence: 0
traits:
  - name: Energy Conservation
    effects:
      - effect: The first time each round that the null is targeted by a strike, it
          takes a bane and the null halves the damage from it. The creature
          making the strike takes 10 damage.
  - name: Rivalry
    effects:
      - effect: At the start of an encounter, the null chooses one creature within their
          line of effect. Both the null and the creature can add a d3 roll to
          power rolls they make against each other.
abilities:
  - name: Kinetic Danse
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
      - roll: Power Roll + 5
        t1: 15 damage; the null shifts up to 4 squares; A < 3 10 damage
        t2: 20 damage; the null shifts up to 5 squares; A < 4 15 damage
        t3: 24 damage; the null shifts up to 6 squares; A < 5 19 damage
  - name: Incapacitate
    icon: 🗡
    cost: 5 Malice
    keywords:
      - Melee
      - Psionic
      - Strike
      - Weapon
    type: Maneuver
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 5
        t1: 13 damage; R < 3 dazed and restrained (save ends)
        t2: 17 damage; R < 4 dazed and restrained (save ends)
        t3: 20 damage; R < 5 dazed and restrained (save ends)
```