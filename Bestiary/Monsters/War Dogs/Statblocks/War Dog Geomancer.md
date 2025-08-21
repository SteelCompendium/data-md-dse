---
agility: 1
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '10'
file_basename: War Dog Geomancer
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 3
intuition: 4
item_id: war-dog-geomancer
item_index: '351'
item_name: War Dog Geomancer
level: 8
might: 2
presence: 2
reason: 4
roles:
- Horde Controller
scc:
- mcdm.monsters.v1:monster:war-dog-geomancer
scdc:
- 1.1.1:2:351
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 3
stamina: '45'
type: monster
---

```ds-statblock
name: War Dog Geomancer
level: 8
roles:
  - Horde Controller
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "10"
stamina: "45"
speed: 5
movement: Burrow
size: 1M
stability: 3
free_strike: 3
might: 2
agility: 1
reason: 4
intuition: 4
presence: 2
traits:
  - name: Dust Cloud
    effects:
      - effect: The geomancer is always surrounded by a 2 aura of swirling dust and
          earthen debris. The geomancer and any ally in the area have
          concealment.
  - name: Loyalty Collar
    effects:
      - effect: When the geomancer is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 3d6 damage to each adjacent enemy and object.
abilities:
  - name: Earthwave
    cost: Signature Ability
    keywords:
      - Area
      - Magic
      - Ranged
    type: Main action
    distance: 7 x 2 line within 10
    target: Each creature in the area
    effects:
      - roll: Power Roll + 4
        t1: 3 damage; M < 2 push (see effect)
        t2: 6 damage; M < 3 push
        t3: 8 damage; M < 4 push, prone
      - effect: This ability ignores stability. The geomancer declares a direction for
          the area, and any creature pushed by this ability is pushed to the
          last space in the area in the chosen direction.
        name: Effect
      - effect: The ground beneath the area becomes a 2-square-deep trench after the
          power roll is resolved
        cost: 2 Malice
  - name: Siegeworks
    keywords:
      - Area
      - Magic
      - Ranged
    type: Maneuver
    distance: 5 wall within 10
    target: Special
    effects:
      - effect: The geomancer raises a wall of stone set with viewing gaps. Creatures
          have line of effect through the wall while adjacent to it.
        name: Effect
```