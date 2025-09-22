---
agility: 1
ancestry:
- Kobold
- Beast
ev: '12'
file_basename: Shieldscale Drangolin
file_dpath: Monsters/Kobolds/Statblocks
free_strike: 5
intuition: 0
item_id: shieldscale-drangolin
item_index: '97'
item_name: Shieldscale Drangolin
level: 1
might: 2
presence: -2
reason: -3
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:shieldscale-drangolin
scdc:
- 1.1.1:2:97
size: 2 or 3
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '80'
type: monster
---

~~~ds-statblock
type: statblock
name: Shieldscale Drangolin
level: 1
roles:
  - Elite Brute
ancestry:
  - Kobold
  - Beast
ev: "12"
stamina: "80"
speed: 7
movement: Burrow
size: 2 or 3
stability: 0
free_strike: 5
might: 2
agility: 1
reason: -3
intuition: 0
presence: -2
features:
  - type: feature
    feature_type: ability
    name: Fiery Claws
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        tier1: 7 fire damage
        tier2: 10 fire damage
        tier3: 13 fire damage
      - name: Special
        effect: If the drangolin is size 3, the distance becomes Melee 2.
  - type: feature
    feature_type: ability
    name: Drangolin Plume
    icon: 👤
    cost: 5 Malice
    keywords:
      - "-"
    usage: Main action
    distance: Self; see below
    target: Self
    effects:
      - name: Effect
        effect: The drangolin shifts up to their speed and uses Fiery Claws against each
          creature who comes adjacent to them during the shift. The drangolin
          makes one power roll against all targets.
  - type: feature
    feature_type: ability
    name: Erupt
    icon: ❇️
    cost: 3 Malice
    keywords:
      - Area
      - Weapon
    usage: Main action
    distance: 2 burst
    target: Each creature in the area
    effects:
      - name: Effect
        effect: The drangolin uses the Dig maneuver to breach the surface before using
          this ability. Each target in the area where the drangolin breaches
          takes an extra 2 fire damage.
      - roll: Power Roll + 2
        tier1: 6 damage; push 1; A < 0 prone
        tier2: 8 damage; push 3; A < 0 prone
        tier3: 11 damage; push 5; A < 0 prone
  - type: feature
    feature_type: trait
    name: Ashen Cloud
    icon: ⭐️
    effects:
      - effect: Any ally adjacent to the drangolin has concealment.
  - type: feature
    feature_type: trait
    name: Burrow Bond
    icon: ⭐️
    effects:
      - effect: When the drangolin burrows, each adjacent size 1S or smaller ally can
          move with them.
~~~