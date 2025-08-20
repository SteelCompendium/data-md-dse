---
agility: 1
ancestry:
- Arixx
- Beast
ev: '36'
file_basename: Arixx
file_dpath: Monsters/Arixx/Statblocks
free_strike: 5
intuition: 1
item_id: arixx
item_index: '237'
item_name: Arixx
level: 1
might: 3
presence: -4
reason: -3
roles:
- Solo
scc:
- mcdm.monsters.v1:monster:arixx
scdc:
- 1.1.1:2:237
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '200'
type: monster
---

```ds-statblock
name: Arixx
level: 1
roles:
  - Solo
ancestry:
  - Arixx
  - Beast
ev: "36"
stamina: "200"
speed: 5
movement: Burrow
size: "2"
stability: 2
free_strike: 5
might: 3
agility: 1
reason: -3
intuition: 1
presence: -4
traits:
  - name: Solo Monster
    effects:
      - effect: At the end of each of their turns, the arixx can take 5 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
        name: End Effect
      - effect: The arixx can take two turns each round. They can't take turns
          consecutively.
        name: Solo Turns
  - name: Earthwalk
    effects:
      - effect: Difficult terrain composed of earth or loose rock doesn't cost the arixx
          extra movement.
  - name: Soft Underbelly
    effects:
      - effect: A prone creature making a melee strike against the arixx has a double
          edge on the strike instead of taking a bane.
abilities:
  - name: Bite
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        t1: 9 damage; grabbed
        t2: 13 damage; grabbed
        t3: 16 damage; grabbed
      - effect: A size 1 target grabbed this way takes 3 acid damage at the start of
          each of their turns.
  - name: Claw Swing
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        t1: 5 damage; A < 1 grabbed
        t2: 8 damage; A < 2 grabbed
        t3: 11 damage; A < 3 grabbed
      - effect: The arixx can vertically slide each grabbed target up to 3 squares.
  - name: Spitfire
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        t1: 4 acid damage
        t2: 6 acid damage
        t3: 7 acid damage; prone
      - effect: The ground beneath each target is covered in burning acid until the end
          of the encounter. Any enemy who enters an affected space for the first
          time in a round or starts their turn there takes 2 acid damage.
  - name: Dirt Devil
    cost: 3 Malice
    keywords:
      - Area
    type: Main action
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        t1: 4 damage
        t2: 6 damage; push 2
        t3: 7 damage; push 4
      - effect: The arixx flings rocks and debris to fill the area, and has a double
          edge on the power roll if they started their turn underground. The
          area is difficult terrain.
  - name: Dust Cloud
    keywords:
      - Area
    type: Maneuver
    distance: 1 burst
    target: Special
    effects:
      - effect: The arixx kicks up dust to fill the area until the start of their next
          turn, then moves up to their speed. Any enemy in the area or who
          targets a creature in the area takes a bane on power rolls.
  - name: Skitter
    keywords:
      - "-"
    type: Triggered action
    distance: Self
    target: Self
    trigger: The arixx takes damage.
    effects:
      - effect: The arixx halves the damage and shifts up to 3 squares after the
          triggering effect resolves.
  - name: Acid Spew
    cost: Villain Action 1
    keywords:
      - Area
      - Weapon
    type: "-"
    distance: 10 x 2 line within 1
    target: Each creature and object in the area
    effects:
      - roll: Power Roll + 3
        t1: 5 acid damage
        t2: 8 acid damage
        t3: 11 acid damage
      - effect: The ground in the area is covered in a puddle of acid until the end of
          the encounter. Any enemy who enters the area for the first time in a
          round or starts their turn there takes 2 acid damage.
  - name: Sinkhole
    cost: Villain Action 2
    keywords:
      - "-"
    type: "-"
    distance: Self
    target: Self
    effects:
      - effect: The arixx shifts up to their speed. If they end this shift above ground
          and within 2 squares of a creature, they use Bite against the creature
          and can then use the Dig maneuver.
  - name: Acid and Claws
    cost: Villain Action 3
    keywords:
      - Area
      - Weapon
    type: "-"
    distance: 2 burst
    target: Each creature in the area
    effects:
      - roll: Power Roll + 3
        t1: 5 acid damage; M < 1 weakened (save ends)
        t2: 8 acid damage; M < 2 weakened (save ends)
        t3: 11 acid damage; M < 3 weakened (save ends)
```