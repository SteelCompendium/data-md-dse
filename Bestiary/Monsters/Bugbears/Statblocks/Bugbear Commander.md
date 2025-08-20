---
agility: 1
ancestry:
- Bugbear
- Fey
- Goblin
- Humanoid
ev: '16'
file_basename: Bugbear Commander
file_dpath: Monsters/Bugbears/Statblocks
free_strike: 5
intuition: 0
item_id: bugbear-commander
item_index: '292'
item_name: Bugbear Commander
level: 2
might: 2
presence: 0
reason: 2
roles:
- Elite Support
scc:
- mcdm.monsters.v1:monster:bugbear-commander
scdc:
- 1.1.1:2:292
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '80'
type: monster
---

```ds-statblock
name: Bugbear Commander
level: 2
roles:
  - Elite Support
ancestry:
  - Bugbear
  - Fey
  - Goblin
  - Humanoid
ev: "16"
stamina: "80"
speed: 5
size: 1L
stability: 0
free_strike: 5
might: 2
agility: 1
reason: 2
intuition: 0
presence: 0
traits:
  - name: The Commander's Watching
    effects:
      - effect: Any ally who has line of effect to the commander can end one condition
          on themself at the start of each of their turns.
abilities:
  - name: Inspiring Swordplay
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
        t1: 7 damage
        t2: 10 damage
        t3: 13 damage; one target is grabbed
      - effect: One ally within 5 squares of the commander gains an edge on their next
          strike until the start of the commander's next turn.
  - name: You Next!
    keywords:
      - Ranged
    type: Main Action
    distance: Ranged 8
    target: One ally
    effects:
      - effect: The target moves up to their speed and uses a signature ability.
  - name: Fall Back!
    cost: 5 Malice
    keywords:
      - Area
    type: Main Action
    distance: 5 burst
    target: Each ally in the area
    effects:
      - effect: Each target shifts up to their speed, then can use the Throw maneuver.
  - name: Throw
    keywords:
      - Melee
      - Strike
    type: Maneuver
    distance: Melee 1
    target: One creature or object
    effects:
      - effect: The target must be grabbed by the commander.
        name: Special
      - effect: The target is vertical pushed up to 4 squares. An ally doesn't take
          damage from being force moved this way.
  - name: Catcher
    keywords:
      - Melee
    type: Free triggered action
    distance: Melee 1
    target: The triggering creature or object
    trigger: A size 1 creature or object is force moved within distance, or a size 1
      ally willingly moves within distance.
    effects:
      - effect: The target is grabbed by the commander.
```