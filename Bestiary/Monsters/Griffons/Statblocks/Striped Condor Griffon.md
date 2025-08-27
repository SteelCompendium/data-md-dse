---
agility: 2
ancestry:
- Beast
- Griffon
ev: '16'
file_basename: Striped Condor Griffon
file_dpath: Monsters/Griffons/Statblocks
free_strike: 5
intuition: 2
item_id: striped-condor-griffon
item_index: '88'
item_name: Striped Condor Griffon
level: 2
might: 2
presence: 1
reason: -1
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:striped-condor-griffon
scdc:
- 1.1.1:2:88
size: '3'
source: mcdm.monsters.v1
speed: 7
stability: 3
stamina: '100'
type: monster
---

```ds-statblock
name: Striped Condor Griffon
level: 2
roles:
  - Elite Brute
ancestry:
  - Beast
  - Griffon
ev: "16"
stamina: "100"
speed: 7
movement: Fly
size: "3"
stability: 3
free_strike: 5
might: 2
agility: 2
reason: -1
intuition: 2
presence: 1
traits:
  - name: Beast of Prey
    effects:
      - effect: While grabbed by the griffon, a creature has a double bane on the Escape
          Grab maneuver.
  - name: Steady
    effects:
      - effect: Any power roll that could knock the griffon prone takes a bane
  - name: Banded Predator
    effects:
      - effect: The griffon can attempt hide even while observed. Additionally, while no
          enemy has line of effect to them, the griffon can attempt to hide at
          the end of their turn
abilities:
  - name: Violent Thrashing
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        t1: 7 damage; push 1
        t2: 11 damage; one target is pushed up to 2 squares; the other target is
          vertical pushed up to 2 squares
        t3: 14 damage; one target is pushed up to 2 squares and knocked prone; the other
          target is vertical pushed up to 3 squares
  - name: Bound Ahead
    icon: 👤
    cost: 5 Malice
    keywords:
      - "-"
    type: Main action
    distance: Self
    target: Self
    effects:
      - effect: The griffon shifts up to their speed along the ground in straight line.
          Each enemy who comes adjacent to the griffon during this shift can
          choose to either take 5 damage or be knocked prone
        name: Effect
  - name: Power Wing Buffet
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
    type: Maneuver
    distance: 5 x 3 line within 1
    target: Each creature or object in the area
    effects:
      - roll: Power Roll + 2
        t1: Push 2; M < 0 the forced movement is vertical
        t2: Push 4; M < 1 the forced movement is vertical
        t3: Push 6; M < 2 the forced movement is vertical
  - name: Circle and Strike
    icon: ❗️
    keywords:
      - Ranged
    type: Triggered action
    distance: Ranged 5
    target: The triggering creature
    trigger: The griffon flies directly above a creature within distance
    effects:
      - effect: The griffon dives down onto the target, taking no damage from falling if
          they reach the ground. The target takes 3 damage for each square the
          griffon dove, and if they have A < 2, they are grabbed or knocked
          prone.
        name: Effect
```