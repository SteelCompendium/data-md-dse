---
agility: 2
ancestry:
- Elemental
ev: '20'
file_basename: Crux of Fire
file_dpath: Monsters/Elementals/Statblocks
free_strike: 6
intuition: 1
item_id: crux-of-fire
item_index: '327'
item_name: Crux of Fire
level: 3
might: -1
presence: 2
reason: 0
roles:
- Elite Artillery
scc:
- mcdm.monsters.v1:monster:crux-of-fire
scdc:
- 1.1.1:2:327
size: 1T
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '80'
type: monster
---

```ds-statblock
name: Crux of Fire
level: 3
roles:
  - Elite Artillery
ancestry:
  - Elemental
ev: "20"
stamina: "80"
immunities:
  - Fire 5
speed: 6
size: 1T
stability: 0
free_strike: 6
might: -1
agility: 2
reason: 0
intuition: 1
presence: 2
traits:
  - name: Fickle and Free
    effects:
      - effect: The crux can't be restrained, slowed, or knocked prone, and they ignore
          difficult terrain.
abilities:
  - name: Spitfire
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 12
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        t1: 8 fire damage
        t2: 12 fire damage; A < 1 the target is burning (save ends)
        t3: 15 fire damage; A < 2 the target is burning (save ends)
      - effect: A burning creature takes 1d6 fire damage at the start of each of their
          turns. A burning object takes 1d6 fire damage at the end of each
          round.
  - name: Convocation of Flames
    keywords:
      - Magic
      - Ranged
    type: Maneuver
    distance: Ranged 5
    target: Self or one elemental
    effects:
      - effect: Until the start of the crux's next turn, the target has fire immunity 5.
      - effect: Until the end of the encounter, the ground within 3 squares of the
          target is wreathed in fire. Any enemy who enters that area for the
          first time in a round or starts their turn there takes 3 fire damage.
        cost: 3 Malice
  - name: Flame Jet
    cost: 1 Malice
    keywords:
      - Magic
    type: Triggered action
    distance: Self
    target: Self
    trigger: The crux takes damage.
    effects:
      - effect: The crux ignores any effects associated with the damage and can fly up
          to their speed. If the crux doesn't end this movement on solid ground,
          they fall.
```