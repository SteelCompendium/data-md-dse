---
agility: 2
ancestry:
- Humanoid
- Rival
ev: '48'
file_basename: Rival Tactician
file_dpath: Monsters/Rivals/4th Echelon/Statblocks
free_strike: 10
intuition: 0
item_id: rival-tactician
item_index: '33'
item_name: Rival Tactician
level: 10
might: 5
presence: 3
reason: 4
roles:
- Elite Artillery
scc:
- mcdm.monsters.v1:monster:rival-tactician
scdc:
- 1.1.1:2:33
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '220'
type: monster
---

```ds-statblock
name: Rival Tactician
level: 10
roles:
  - Elite Artillery
ancestry:
  - Humanoid
  - Rival
ev: "48"
stamina: "220"
speed: 5
size: 1M
stability: 2
free_strike: 10
might: 5
agility: 2
reason: 4
intuition: 0
presence: 3
traits:
  - name: Rivalry
    effects:
      - effect: At the start of an encounter, the tactician chooses one creature within
          their line of effect. Both the tactician and the creature can add a d3
          roll to power rolls they make against each other.
abilities:
  - name: Forward Assault
    cost: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 5
        t1: 15 damage
        t2: 21 damage; A < 4 prone and can't stand (EoT)
        t3: 25 damage; prone; A < 5 can't stand (EoT)
      - effect: Two allies within distance move up to their speed and can use a
          signature ability that has a double edge.
        cost: 5 Malice
  - name: Guardian From Afar
    cost: 3 Malice
    keywords:
      - Area
      - Ranged
      - Weapon
    type: Main action
    distance: 3 cube within 10
    target: One creature in the area
    effects:
      - roll: Power Roll + 5
        t1: 10 damage; M < 3 weakened (save ends)
        t2: 16 damage; M < 4 weakened (save ends)
        t3: 20 damage; M < 5 weakened (save ends)
      - effect: Each ally in the area regains 10 Stamina.
  - name: Battlefield Control
    keywords:
      - Ranged
    type: Triggered action
    distance: Ranged 10
    target: The triggering enemy
    trigger: An enemy within distance willingly moves.
    effects:
      - effect: At any point during the movement, the tactician and one ally within
          distance can use a signature ability against the target.
```