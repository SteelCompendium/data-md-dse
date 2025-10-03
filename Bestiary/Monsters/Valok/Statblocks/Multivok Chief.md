---
agility: 1
ancestry:
- Construct
- Multivok
- Soulless
- Valok
ev: '44'
file_basename: Multivok Chief
file_dpath: Monsters/Valok/Statblocks
free_strike: 9
intuition: 1
item_id: multivok-chief
item_index: '330'
item_name: Multivok Chief
level: 9
might: 4
presence: -3
reason: -2
roles:
- Elite Support
scc:
- mcdm.monsters.v1:monster:multivok-chief
scdc:
- 1.1.1:2:330
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 3
stamina: '220'
type: monster
---

~~~ds-statblock
type: statblock
name: Multivok Chief
level: 9
roles:
  - Elite Support
ancestry:
  - Construct
  - Multivok
  - Soulless
  - Valok
ev: "44"
stamina: "220"
speed: 5
size: 1L
stability: 3
free_strike: 9
might: 4
agility: 1
reason: -2
intuition: 1
presence: -3
features:
  - type: feature
    feature_type: ability
    name: Pneumatic Punch
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        tier1: 13 damage; push 3
        tier2: 18 damage; push 5
        tier3: 22 damage; push 8
  - type: feature
    feature_type: ability
    name: Targeting Beam
    icon: 🏹
    cost: 3 Malice
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        tier1: 15 damage; A < 2 slowed (save ends)
        tier2: 21 damage; A < 3 slowed (save ends)
        tier3: 26 damage; A < 4 slowed (save ends)
      - name: Effect
        effect: This damage can't be reduced in any way. While a target is slowed this
          way, any strike against them has a double edge.
  - type: feature
    feature_type: ability
    name: Chief's Command
    icon: 🏹
    keywords:
      - Ranged
    usage: Maneuver
    distance: Ranged 5
    target: One ally
    effects:
      - name: Effect
        effect: The target shifts up to their speed and can use a main action.
  - type: feature
    feature_type: ability
    name: Quick Shield
    icon: ❗️
    keywords:
      - Ranged
    usage: Triggered action
    distance: Ranged 10
    target: The triggering creature
    trigger: The chief or an ally within distance is subject to an effect that can
      be ended by a saving throw or that ends at the end of their turn.
    effects:
      - name: Effect
        effect: The target gains 15 temporary Stamina. Each time this triggered action
          is used, the amount of temporary Stamina received decreases by 3 (to a
          minimum of 0).
  - type: feature
    feature_type: trait
    name: Multivok Maintenance
    icon: ⭐️
    effects:
      - effect: At the start of the chief's turn, each servok within 2 squares of them
          regains 15 Stamina.
  - type: feature
    feature_type: trait
    name: Crafted to Perfection
    icon: ⭐️
    effects:
      - effect: The chief's shape can't be changed by any external effect.
  - type: feature
    feature_type: trait
    name: Valiar Might
    icon: ⭐️
    effects:
      - effect: While the chief isn't bleeding, weakened, or winded, any power roll made
          against them is automatically a tier 1 outcome. A critical hit still
          grants its additional main action.
~~~