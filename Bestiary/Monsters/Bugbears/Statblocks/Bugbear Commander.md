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
item_index: '290'
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
- 1.1.1:2:290
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '80'
type: monster
---

~~~ds-statblock
type: statblock
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
features:
  - type: feature
    feature_type: ability
    name: Inspiring Swordplay
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        tier1: 7 damage
        tier2: 10 damage
        tier3: 13 damage; one target is grabbed
      - name: Effect
        effect: One ally within 5 squares of the commander gains an edge on their next
          strike until the start of the commander's next turn.
  - type: feature
    feature_type: ability
    name: You Next!
    icon: 🏹
    keywords:
      - Ranged
    usage: Main Action
    distance: Ranged 8
    target: One ally
    effects:
      - name: Effect
        effect: The target moves up to their speed and uses a signature ability.
  - type: feature
    feature_type: ability
    name: Fall Back!
    icon: ❇️
    cost: 5 Malice
    keywords:
      - Area
    usage: Main Action
    distance: 5 burst
    target: Each ally in the area
    effects:
      - name: Effect
        effect: Each target shifts up to their speed, then can use the Throw maneuver.
  - type: feature
    feature_type: ability
    name: Throw
    icon: 🗡
    keywords:
      - Melee
      - Strike
    usage: Maneuver
    distance: Melee 1
    target: One creature or object
    effects:
      - name: Special
        effect: The target must be grabbed by the commander.
      - name: Effect
        effect: The target is vertical pushed up to 4 squares. An ally doesn't take
          damage from being force moved this way.
  - type: feature
    feature_type: ability
    name: Catcher
    icon: ❗️
    keywords:
      - Melee
    usage: Free triggered action
    distance: Melee 1
    target: The triggering creature or object
    trigger: A size 1 creature or object is force moved within distance, or a size 1
      ally willingly moves within distance.
    effects:
      - name: Effect
        effect: The target is grabbed by the commander.
  - type: feature
    feature_type: trait
    name: The Commander's Watching
    icon: ⭐️
    effects:
      - effect: Any ally who has line of effect to the commander can end one condition
          on themself at the start of each of their turns.
~~~