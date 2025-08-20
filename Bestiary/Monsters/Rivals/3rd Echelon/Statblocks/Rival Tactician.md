---
agility: 1
ancestry:
- Humanoid
- Rival
ev: '40'
file_basename: Rival Tactician
file_dpath: Monsters/Rivals/3rd Echelon/Statblocks
free_strike: 9
intuition: 0
item_id: rival-tactician
item_index: '26'
item_name: Rival Tactician
level: 8
might: 4
presence: 2
reason: 3
roles:
- Elite Artillery
scc:
- mcdm.monsters.v1:monster:rival-tactician
scdc:
- 1.1.1:2:26
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '180'
type: monster
---

```ds-statblock
name: Rival Tactician
level: 8
roles:
  - Elite Artillery
ancestry:
  - Humanoid
  - Rival
ev: "40"
stamina: "180"
speed: 5
size: 1M
stability: 2
free_strike: 9
might: 4
agility: 1
reason: 3
intuition: 0
presence: 2
traits:
  - name: Rivalry
    effects:
      - effect: At the start of an encounter, the tactician chooses one creature within
          their line of effect. Both the tactician and the creature can add a d3
          roll to power rolls they make against each other.
abilities:
  - name: Command From the Back
    cost: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        t1: 13 damage
        t2: 18 damage; A < 3 prone
        t3: 22 damage; A < 4 prone
      - effect: Two allies within distance move up to their speed and can use a
          signature ability.
        cost: 4 Malice
  - name: Safeguard
    cost: 3 Malice
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        t1: 15 damage; M < 2 weakened (save ends)
        t2: 21 damage; M < 3 weakened (save ends)
        t3: 26 damage; M < 4 weakened (save ends)
      - effect: Two allies adjacent to the target each regain 7 Stamina.
  - name: Quickshot
    keywords:
      - Ranged
    type: Triggered action
    distance: Ranged 10
    target: The triggering enemy
    trigger: An enemy within distance willingly moves.
    effects:
      - effect: At any point during the movement, the tactician uses a signature ability
          against the target.
```