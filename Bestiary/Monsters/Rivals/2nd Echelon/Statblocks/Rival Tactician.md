---
agility: 0
ancestry:
- Humanoid
- Rival
ev: '28'
file_basename: Rival Tactician
file_dpath: Monsters/Rivals/2nd Echelon/Statblocks
free_strike: 7
intuition: 0
item_id: rival-tactician
item_index: '19'
item_name: Rival Tactician
level: 5
might: 3
presence: 1
reason: 2
roles:
- Elite Artillery
scc:
- mcdm.monsters.v1:monster:rival-tactician
scdc:
- 1.1.1:2:19
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '120'
type: monster
---

```ds-statblock
name: Rival Tactician
level: 5
roles:
  - Elite Artillery
ancestry:
  - Humanoid
  - Rival
ev: "28"
stamina: "120"
speed: 5
size: 1M
stability: 2
free_strike: 7
might: 3
agility: 0
reason: 2
intuition: 0
presence: 1
traits:
  - name: Rivalry
    effects:
      - effect: At the start of an encounter, the tactician chooses one creature within
          their line of effect. Both the tactician and the creature can add a d3
          roll to power rolls they make against each other.
abilities:
  - name: Mark Targets
    cost: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        t1: 10 damage
        t2: 15 damage
        t3: 18 damage
      - effect: Two allies within distance can use a signature ability against the same
          target.
        cost: 3 Malice
  - name: Preserve and Protect
    cost: 3 Malice
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 5
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        t1: 11 damage; M < 1 weakened (save ends)
        t2: 16 damage; M < 2 weakened (save ends)
        t3: 21 damage; M < 3 weakened (save ends)
      - effect: One ally adjacent to the target regains 7 Stamina.
  - name: Take the Opening
    keywords:
      - Ranged
    type: Triggered action
    distance: Ranged 10
    target: The triggering enemy
    trigger: An enemy within distance willingly moves.
    effects:
      - effect: At any point during the movement, the tactician and one ally within
          distance can each make a free strike against the target.
```