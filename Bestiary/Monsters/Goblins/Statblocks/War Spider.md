---
agility: 1
ancestry:
- Animal
- Goblin
ev: '12'
file_basename: War Spider
file_dpath: Monsters/Goblins/Statblocks
free_strike: 4
intuition: 0
item_id: war-spider
item_index: '314'
item_name: War Spider
level: 1
might: 2
presence: -3
reason: -4
roles:
- Elite Mount
scc:
- mcdm.monsters.v1:monster:war-spider
scdc:
- 1.1.1:2:314
size: '3'
source: mcdm.monsters.v1
speed: 7
stability: 2
stamina: '60'
type: monster
---

```ds-statblock
name: War Spider
level: 1
roles:
  - Elite Mount
ancestry:
  - Animal
  - Goblin
ev: "12"
stamina: "60"
speed: 7
movement: Climb
size: "3"
stability: 2
free_strike: 4
might: 2
agility: 1
reason: -4
intuition: 0
presence: -3
traits:
  - name: Ride Launcher
    effects:
      - effect: Any ally who leaps off the back of the spider can jump up to 6 squares
          without making a test, and takes no damage if they fall during the
          jump. After any ally jumps, the first melee strike the make on the
          same turn gains an edge.
  - name: Wide Back
    effects:
      - effect: While riding the spider, two size 1 allies can occupy the same space
abilities:
  - name: Bite
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature
    effects:
      - roll: Power Roll + 2
        t1: 7 poison damage
        t2: 11 poison damage
        t3: 14 poison damage; M < 2 weakened (save ends)
      - effect: For any tier outcome, if the target has M < 3, they are weakened (save
          ends).
        cost: 2 Malice
  - name: Leg Blade
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        t1: 6 damage
        t2: 9 damage
        t3: 12 damage
  - name: Trample
    cost: 5 Malice
    keywords:
      - "-"
    type: Main action
    distance: Self
    target: Self
    effects:
      - effect: The spider shifts up to their speed and uses Leg Blade against each
          creature who comes adjacent to them during the shift. The spider makes
          one power roll against all targets.
        name: Effect
  - name: Web
    keywords:
      - Area
      - Weapon
    type: Maneuver
    distance: 3 cube within 1
    target: Each creature in the area
    effects:
      - roll: Power Roll + 2
        t1: A < 0 restrained (save ends)
        t2: A < 1 restrained (save ends)
        t3: A < 2 restrained (save ends)
      - effect: The area is difficult terrain for enemies.
        name: Effect
  - name: Skitter
    keywords:
      - "-"
    type: Triggered action
    distance: Self
    target: Self
    trigger: The spider or any ally riding the spider takes damage.
    effects:
      - effect: The damage is halved, and the spider shifts up to 2 squares after the
          triggering effect resolve
        name: Effect
```