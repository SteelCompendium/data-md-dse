---
agility: 1
ancestry:
- Giant
- Stone Giant
ev: '40'
file_basename: Granite Stone Giant
file_dpath: Monsters/Giants/Statblocks
free_strike: 8
intuition: 2
item_id: granite-stone-giant
item_index: '204'
item_name: Granite Stone Giant
level: 8
might: 4
presence: 1
reason: 1
roles:
- Elite Defender
scc:
- mcdm.monsters.v1:monster:granite-stone-giant
scdc:
- 1.1.1:2:204
size: '4'
source: mcdm.monsters.v1
speed: 7
stability: 10
stamina: '247'
type: monster
---

```ds-statblock
name: Granite Stone Giant
level: 8
roles:
  - Elite Defender
ancestry:
  - Giant
  - Stone Giant
ev: "40"
stamina: "247"
speed: 7
movement: Burrow
size: "4"
stability: 10
free_strike: 8
might: 4
agility: 1
reason: 1
intuition: 2
presence: 1
traits:
  - name: Stonebreaker Flesh
    effects:
      - effect: Whenever an enemy obtains a tier 1 outcome on a melee ability used
          against the granite stone giant, they take a bane on that ability
          until the end of the encounter.
  - name: Stone Steps
    effects:
      - effect: The granite stone giant ignores difficult terrain.
  - name: Stone Swim
    effects:
      - effect: The granite stone giant can burrow through stone, but can't drag other
          creatures underground when they do so.
abilities:
  - name: Jagged Stone Club
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 3
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        t1: 12 damage
        t2: 17 damage; R < 3 weakened (save ends)
        t3: 21 damage; R < 4 weakened (save ends)
      - effect: If the target is already weakened, they are also bleeding (save ends).
  - name: Crag Burst
    cost: 3 Malice
    keywords:
      - Area
    type: Main action
    distance: 2 burst
    target: Each enemy and object in the area
    effects:
      - roll: Power Roll + 4
        t1: 6 damage; push 2
        t2: 10 damage; push 4
        t3: 14 damage; vertical push 4
      - effect: The area is difficult terrain. Whenever a creature enters square in the
          area, they take 3 damage.
  - name: Castle Stone Shape
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The granite stone giant moves up to their speed and creates a 14 wall of
          stone in squares adjacent to the path of their movement.
  - name: Pillar
    keywords:
      - Melee
    type: Triggered action
    distance: Melee 3
    target: The triggering creature or object
    trigger: A creature or object within distance moves or shifts away from the
      granite stone giant.
    effects:
      - effect: A 1-square pillar of stone rises 5 squares out of the ground beneath the
          target, who moves with the ground to its new elevation, then is
          vertical pushed 5 squares.
```