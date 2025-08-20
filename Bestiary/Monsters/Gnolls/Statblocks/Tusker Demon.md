---
agility: -1
ancestry:
- Abyssal
- Demon
- Gnoll
ev: '16'
file_basename: Tusker Demon
file_dpath: Monsters/Gnolls/Statblocks
free_strike: 5
intuition: 0
item_id: tusker-demon
item_index: '41'
item_name: Tusker Demon
level: 2
might: 2
presence: -1
reason: -3
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:tusker-demon
scdc:
- 1.1.1:2:41
size: '3'
source: mcdm.monsters.v1
speed: 7
stability: 3
stamina: '100'
type: monster
---

```ds-statblock
name: Tusker Demon
level: 2
roles:
  - Elite Brute
ancestry:
  - Abyssal
  - Demon
  - Gnoll
ev: "16"
stamina: "100"
speed: 7
size: "3"
stability: 3
free_strike: 5
might: 2
agility: -1
reason: -3
intuition: 0
presence: -1
traits:
  - name: Trample
    effects:
      - effect: The tusker demon can move through enemies' spaces at their usual speed.
          When the tusker enters a creature's space for the first time on a
          turn, that creature takes 5 damage. The tusker demon can end their
          turn in a prone size 1 creature's space, preventing the creature from
          standing up.
  - name: Lethe
    effects:
      - effect: While the tusker demon is winded, they gain an edge on strikes, and any
          strike made against them gains an edge
abilities:
  - name: Gore
    cost: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        t1: 7 damage; push 1
        t2: 11 damage; push 2
        t3: 14 damage; push 3, prone
      - effect: If this ability is used as part of the Charge main action, it deals an
          extra 4 damage.
  - name: Vengeful Tusker
    keywords:
      - Ranged
    type: Triggered action
    distance: Ranged 7
    target: The triggering enemy
    trigger: An enemy within distance deals damage to the tusker.
    effects:
      - effect: The tusker demon uses the Charge main action and Gore against the
          target.
```