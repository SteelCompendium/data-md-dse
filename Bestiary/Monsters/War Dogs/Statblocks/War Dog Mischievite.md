---
agility: 3
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '7'
file_basename: War Dog Mischievite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 3
intuition: 2
item_id: war-dog-mischievite
item_index: '381'
item_name: War Dog Mischievite
level: 5
might: 1
presence: 0
reason: 0
roles:
- Horde Harrier
scc:
- mcdm.monsters.v1:monster:war-dog-mischievite
scdc:
- 1.1.1:2:381
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '35'
type: monster
---

~~~ds-statblock
type: statblock
name: War Dog Mischievite
level: 5
roles:
  - Horde Harrier
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "7"
stamina: "35"
speed: 6
size: 1M
stability: 0
free_strike: 3
might: 1
agility: 3
reason: 0
intuition: 2
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Fuse-Iron Knives
    icon: ⚔️
    ability_type: Signature Ability
    keywords:
      - Melee
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1 or ranged 5
    target: Two creatures
    effects:
      - roll: Power Roll + 3
        tier1: 5 damage
        tier2: 7 damage
        tier3: 8 damage; R < 3 the target is dazzled (save ends)
      - name: Effect
        effect: A dazzled target takes a bane on strikes and has line of effect only
          within 1 square.
  - type: feature
    feature_type: ability
    name: Misdirection
    icon: 🏹
    keywords:
      - Ranged
    usage: Maneuver
    distance: Ranged 3
    target: One ally or dazzled creature
    effects:
      - name: Effect
        effect: The mischievite swaps positions with the target. An ally targeted by
          this ability can make a free strike before or after being swapped.
      - cost: 2 Malice
        effect: The mischievite can use this ability as a triggered action when they are
          targeted by an ability. If they do, the swapped target becomes the new
          target of the triggering ability.
  - type: feature
    feature_type: trait
    name: Crafty
    icon: ⭐️
    effects:
      - effect: The mischievite doesn't provoke opportunity attacks by moving.
  - type: feature
    feature_type: trait
    name: Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When the mischievite is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 2d6 damage to each adjacent enemy and object.
~~~