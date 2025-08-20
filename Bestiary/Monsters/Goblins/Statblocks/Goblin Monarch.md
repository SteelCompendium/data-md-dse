---
agility: 3
ancestry:
- Goblin
- Humanoid
ev: '12'
file_basename: Goblin Monarch
file_dpath: Monsters/Goblins/Statblocks
free_strike: 4
intuition: 0
item_id: goblin-monarch
item_index: '309'
item_name: Goblin Monarch
level: 1
might: 0
presence: 3
reason: 1
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:goblin-monarch
scdc:
- 1.1.1:2:309
size: 1S
source: mcdm.monsters.v1
speed: 6
stability: 1
stamina: '80'
type: monster
---

```ds-statblock
name: Goblin Monarch
level: 1
roles:
  - Leader
ancestry:
  - Goblin
  - Humanoid
ev: "12"
stamina: "80"
speed: 6
movement: Climb
size: 1S
stability: 1
free_strike: 4
might: 0
agility: 3
reason: 1
intuition: 0
presence: 3
traits:
  - name: Crafty
    effects:
      - effect: The monarch doesn't provoke opportunity attacks by moving.
  - name: End Effect
    effects:
      - effect: At the end of each of their turns, the monarch can take 5 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
abilities:
  - name: Handaxe
    cost: Signature Ability
    keywords:
      - Melee
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1 or ranged 5
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        t1: 7 damage
        t2: 10 damage
        t3: 13 damage
      - effect: One ally within 10 squares of the monarch can make a free strike.
  - name: Get in Here!
    cost: 1 Malice
    keywords:
      - Ranged
    type: Maneuver
    distance: Ranged 20
    target: Special
    effects:
      - effect: Two goblin runners appear in unoccupied spaces within distance.
  - name: Meat Shield
    keywords:
      - Melee
    type: Triggered action
    distance: Melee 1
    target: One ally
    trigger: A creature targets the monarch with a strike.
    effects:
      - effect: The ally is the target of the triggering strike instead
  - name: What Are You Waiting For?
    cost: Villain Action 1
    keywords:
      - Area
    type: "-"
    distance: 10 burst
    target: Each ally in the area
    effects:
      - effect: Each target can move up to their speed or make a free strike.
  - name: Focus Fire
    cost: Villain Action 2
    keywords:
      - Ranged
    type: "-"
    distance: Ranged 10
    target: One enemy or object
    effects:
      - effect: Each ally within 10 squares of the target can move up to their speed
          toward the target.
  - name: Kill!
    cost: Villain Action 3
    keywords:
      - "-"
    type: "-"
    distance: Special
    target: Special
    effects:
      - effect: Each enemy in the encounter takes 2 damage for each goblin adjacent to
          them.
```