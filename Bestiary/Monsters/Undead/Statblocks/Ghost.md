---
agility: 2
ancestry:
- Undead
ev: '12'
file_basename: Ghost
file_dpath: Monsters/Undead/Statblocks
free_strike: 4
intuition: 0
item_id: ghost
item_index: '80'
item_name: Ghost
level: 1
might: -2
presence: 3
reason: 0
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:ghost
scdc:
- 1.1.1:2:80
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 1
stamina: '80'
type: monster
---

```ds-statblock
name: Ghost
level: 1
roles:
  - Leader
ancestry:
  - Undead
ev: "12"
stamina: "80"
immunities:
  - Corruption 3
  - poison 3
speed: 6
movement: Fly, hover
size: 1M
stability: 1
free_strike: 4
might: -2
agility: 2
reason: 0
intuition: 0
presence: 3
traits:
  - name: Phantom Flow
    effects:
      - effect: Each undead with a Phasing trait within 10 squares of the ghost can't be
          made slowed or weakened.
  - name: Corruptive Phasing
    effects:
      - effect: The ghost can move through creatures and objects at their usual speed,
          but can't end their turn inside a creature or object. The first time
          in a round that the ghost moves through a creature, that creature
          takes 2 corruption damage. The ghost doesn't take damage from being
          force moved into objects.
abilities:
  - name: Heat Death
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 5
    target: Two creatures
    effects:
      - roll: Power Roll + 3
        t1: 7 cold damage; P < 1 slowed (save ends)
        t2: 10 cold damage; P < 2 slowed (save ends)
        t3: 13 cold damage; P < 3 slowed (save ends)
      - effect: The next strike made against the target gains an edge.
  - name: Haunt
    keywords:
      - Ranged
    type: Maneuver
    distance: Ranged 8
    target: Self or one ally with a Phasing trait
    effects:
      - effect: The target shifts up to their speed
      - effect: The ghost chooses one additional target.
        cost: 2 Malice
  - name: Shriek
    cost: 1 Malice
    keywords:
      - Magic
      - Melee
    type: Triggered action
    distance: Melee 1
    target: The triggering creature
    trigger: A creature within distance targets the ghost with a strike.
    effects:
      - effect: The ghost halves the damage from the strike and the target takes 2 sonic
          damage.
  - name: Paranormal Activity
    cost: Villain Action 1
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 5 burst
    target: Each size 3 or smaller object in the area
    effects:
      - effect: Each target rises 1 square into the air and is vertically pulled up to 5
          squares toward the nearest enemy within 3 squares of the target.
  - name: Spirited Away
    cost: Villain Action 2
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        t1: P < 1 the target is levitated (EoT)
        t2: P < 2 the target is levitated (EoT)
        t3: P < 3 the target is levitated until the end of the encounter
      - effect: A levitated target floats 1 square off the ground when first affected,
          then rises 1 square at the end of each of their turns. If a levitated
          target can't already fly, they can fly but are slowed and weakened
          while flying this way
  - name: Awful Wail
    cost: Villain Action 3
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        t1: 3 sonic damage
        t2: 5 sonic damage
        t3: 8 sonic damage
      - effect: A target who has P < 2 is reduced to 1 Stamina if they are winded after
          taking this damage.
```