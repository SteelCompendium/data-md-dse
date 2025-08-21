---
agility: 4
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '10'
file_basename: War Dog Aerocite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 3
intuition: 3
item_id: war-dog-aerocite
item_index: '366'
item_name: War Dog Aerocite
level: 8
might: 0
presence: 1
reason: 1
roles:
- Horde Harrier
scc:
- mcdm.monsters.v1:monster:war-dog-aerocite
scdc:
- 1.1.1:2:366
size: 1M
source: mcdm.monsters.v1
speed: 8
stability: 0
stamina: '50'
type: monster
---

```ds-statblock
name: War Dog Aerocite
level: 8
roles:
  - Horde Harrier
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "10"
stamina: "50"
speed: 8
movement: Fly
size: 1M
stability: 0
free_strike: 3
might: 0
agility: 4
reason: 1
intuition: 3
presence: 1
traits:
  - name: Jetwing Agility
    effects:
      - effect: If the aerocite moves 5 or more squares on their turn, strikes made
          against them take a bane until the start of their next turn.
  - name: Loyalty Collar
    effects:
      - effect: When the aerocite is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 3d6 damage to each adjacent enemy and object.
abilities:
  - name: Dive Bomb
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        t1: 7 damage
        t2: 10 damage; vertical slide 2
        t3: 12 damage; vertical slide 3
      - effect: An enemy force moved by this ability is grabbed instead.
        cost: 1 Malice
  - name: Caustic Paste Bomb
    cost: 2 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    type: Maneuver
    distance: 3 cube within 5
    target: Each creature or object in the area
    effects:
      - roll: Power Roll + 4
        t1: 2 acid damage; M < 2 slowed (save ends)
        t2: 4 acid damage; M < 3 slowed (save ends)
        t3: 6 acid damage; M < 4 slowed (save ends)
      - effect: The area is difficult terrain
        name: Effect
```