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
item_index: '325'
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
- 1.1.1:2:325
size: 1T
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '80'
type: monster
---

~~~ds-statblock
type: statblock
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
features:
  - type: feature
    feature_type: ability
    name: Spitfire
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 12
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        tier1: 8 fire damage
        tier2: 12 fire damage; A < 1 the target is burning (save ends)
        tier3: 15 fire damage; A < 2 the target is burning (save ends)
      - name: Effect
        effect: A burning creature takes 1d6 fire damage at the start of each of their
          turns. A burning object takes 1d6 fire damage at the end of each
          round.
  - type: feature
    feature_type: ability
    name: Convocation of Flames
    icon: 🏹
    keywords:
      - Magic
      - Ranged
    usage: Maneuver
    distance: Ranged 5
    target: Self or one elemental
    effects:
      - name: Effect
        effect: Until the start of the crux's next turn, the target has fire immunity 5.
      - cost: 3 Malice
        effect: Until the end of the encounter, the ground within 3 squares of the
          target is wreathed in fire. Any enemy who enters that area for the
          first time in a round or starts their turn there takes 3 fire damage.
  - type: feature
    feature_type: ability
    name: Flame Jet
    icon: ❗️
    cost: 1 Malice
    keywords:
      - Magic
    usage: Triggered action
    distance: Self
    target: Self
    trigger: The crux takes damage.
    effects:
      - name: Effect
        effect: The crux ignores any effects associated with the damage and can fly up
          to their speed. If the crux doesn't end this movement on solid ground,
          they fall.
  - type: feature
    feature_type: trait
    name: Fickle and Free
    icon: ⭐️
    effects:
      - effect: The crux can't be restrained, slowed, or knocked prone, and they ignore
          difficult terrain.
~~~