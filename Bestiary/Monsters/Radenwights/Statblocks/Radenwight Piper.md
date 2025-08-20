---
agility: 0
ancestry:
- Humanoid
- Radenwight
ev: '6'
file_basename: Radenwight Piper
file_dpath: Monsters/Radenwights/Statblocks
free_strike: 3
intuition: 2
item_id: radenwight-piper
item_index: '150'
item_name: Radenwight Piper
level: 1
might: 0
presence: 1
reason: 0
roles:
- Platoon Support
scc:
- mcdm.monsters.v1:monster:radenwight-piper
scdc:
- 1.1.1:2:150
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '30'
type: monster
---

```ds-statblock
name: Radenwight Piper
level: 1
roles:
  - Platoon Support
ancestry:
  - Humanoid
  - Radenwight
ev: "6"
stamina: "30"
speed: 5
movement: Climb
size: 1S
stability: 0
free_strike: 3
might: 0
agility: 0
reason: 0
intuition: 2
presence: 1
traits:
  - name: Musical Suggestion
    effects:
      - effect: At the end of the piper's turn, they can slide one adjacent creature up
          to 2 squares, ignoring stability.
abilities:
  - name: Piercing Trill
    cost: Signature Ability
    keywords:
      - Magic
      - Melee
      - Ranged
      - Strike
    type: Main action
    distance: Melee 1 or ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 5 sonic damage; push 1
        t2: 7 sonic damage; push 3
        t3: 9 sonic damage; push 4
      - effect: The piper or one ally within distance regains Stamina equal to the
          damage dealt.
  - name: Vivace Vivace!
    keywords:
      - Area
      - Magic
    type: Maneuver
    distance: 3 burst
    target: Each ally in the area
    effects:
      - effect: Each target who has used their Ready Rodent ability this round regains
          the use of their triggered action.
      - effect: The area increases to a 6 burst.
        cost: 2 Malice
  - name: Ready Rodent
    keywords:
      - Melee
      - Weapon
    type: Triggered action
    distance: Melee 1
    target: One creature
    trigger: An ally deals damage to the target.
    effects:
      - effect: The piper makes a free strike against the target.
```