---
agility: -2
ancestry:
- Soulless
- War Dog
ev: '10'
file_basename: War Dog Ballistite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 4
intuition: 3
item_id: war-dog-ballistite
item_index: '360'
item_name: War Dog Ballistite
level: 8
might: 4
presence: 2
reason: 2
roles:
- Horde Artillery
scc:
- mcdm.monsters.v1:monster:war-dog-ballistite
scdc:
- 1.1.1:2:360
size: 1L
source: mcdm.monsters.v1
speed: 0
stability: 5
stamina: '72'
type: monster
---

~~~ds-statblock
type: statblock
name: War Dog Ballistite
level: 8
roles:
  - Horde Artillery
ancestry:
  - Soulless
  - War Dog
ev: "10"
stamina: "72"
speed: 0
size: 1L
stability: 5
free_strike: 4
might: 4
agility: -2
reason: 2
intuition: 3
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Biokinetic Ballista
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 15
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        tier1: 7 damage; push 1
        tier2: 10 damage; push 3
        tier3: 11 damage; push 5
      - name: Effect
        effect: Any target pushed into an obstacle is knocked prone, and if they have M
          < 3 they are restrained (save ends).
  - type: feature
    feature_type: ability
    name: Kill Zone
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    usage: Maneuver
    distance: 3 cube within 12
    target: Special
    effects:
      - name: Effect
        effect: Until the start of the ballistite's next turn, the area is difficult
          terrain, and any ranged ability targeting an enemy in the area deals
          an extra 8 damage.
  - type: feature
    feature_type: trait
    name: Set Up and Tear Down
    icon: ⭐️
    effects:
      - effect: At the start of each of the ballistite's turns, they can gain a +4 bonus
          to speed until the end of their turn. While their speed is greater
          than 0 by any means, they can't use main actions or maneuvers.
  - type: feature
    feature_type: trait
    name: Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When the ballistite is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 3d6 damage to each adjacent enemy and object.
~~~