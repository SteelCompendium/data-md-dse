---
agility: 3
ancestry:
- Humanoid
- Time Raider
ev: '20'
file_basename: Time Raider Tyrannis
file_dpath: Monsters/Time Raiders/Statblocks
free_strike: 5
intuition: 1
item_id: time-raider-tyrannis
item_index: '139'
item_name: Time Raider Tyrannis
level: 3
might: 0
presence: 0
reason: 3
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:time-raider-tyrannis
scdc:
- 1.1.1:2:139
size: '2'
source: mcdm.monsters.v1
speed: 1
stability: 2
stamina: '0120'
type: monster
---

```ds-statblock
name: Time Raider Tyrannis
level: 3
roles:
  - Leader
ancestry:
  - Humanoid
  - Time Raider
ev: "20"
stamina: "0120"
immunities:
  - Psychic 5
speed: 1
movement: Hover, teleport
size: "2"
stability: 2
free_strike: 5
might: 0
agility: 3
reason: 3
intuition: 1
presence: 0
traits:
  - name: End Effect
    effects:
      - effect: At the end of each of their turns, the tyrannis can take 5 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
  - name: Foresight
    effects:
      - effect: The tyrannis doesn't take a bane on strikes against creatures with
          concealment.
abilities:
  - name: Gatling Blaster
    cost: Signature Ability
    keywords:
      - Melee
      - Psionic
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2 or ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        t1: 8 corruption damage
        t2: 12 corruption damage
        t3: 15 corruption damage
      - effect: Each target takes a −2 penalty to speed until the start of the
          tyrannis's next turn.
  - name: Air Raid!
    cost: 3 Malice
    keywords:
      - Psionic
      - Ranged
    type: Maneuver
    distance: Ranged 10
    target: Three time raiders
    effects:
      - effect: Each target can fly up to their speed and make a free strike. If a
          target doesn't land in an unoccupied space, they fall.
  - name: Precog Reflexes
    keywords:
      - Psionic
      - Ranged
    type: Triggered action
    distance: Ranged 10
    target: The triggering creature
    trigger: A creature within distance makes a strike against the tyrannis.
    effects:
      - effect: The strike takes a bane. After the strike resolves, the tyrannis can
          make a free strike against the target.
      - effect: The strike has a double bane instead.
        cost: 2 Malice
  - name: We Will Won!
    cost: Villain Action 1
    keywords:
      - Psionic
      - Ranged
    type: "-"
    distance: Ranged 10
    target: Self and three allies
    effects:
      - effect: Each target gains 15 temporary Stamina, and has their speed doubled
          until the end of their next turn.
  - name: Stick to the Plan!
    cost: Villain Action 2
    keywords:
      - Area
    type: "-"
    distance: 10 burst
    target: Self and each ally in the area
    effects:
      - effect: Each target can end one effect on them or can move up to their speed.
  - name: Armageddon
    cost: Villain Action 3
    keywords:
      - Area
    type: "-"
    distance: 5 burst
    target: Special
    effects:
      - effect: The tyrannis fires a sensor mine into each unoccupied square in the
          area, and creates a gravity well whose area contains one or more
          squares of the tyrannis's space (see Gravity Well). Whenever an enemy
          enters a square with a sensor mine in it, the mine explodes, dealing 3
          damage to the enemy.
```