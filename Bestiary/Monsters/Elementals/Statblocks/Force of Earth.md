---
agility: -1
ancestry:
- Elemental
ev: '20'
file_basename: Force of Earth
file_dpath: Monsters/Elementals/Statblocks
free_strike: 6
intuition: 1
item_id: force-of-earth
item_index: '324'
item_name: Force of Earth
level: 3
might: 2
presence: 2
reason: 0
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:force-of-earth
scdc:
- 1.1.1:2:324
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '132'
type: monster
---

~~~ds-statblock
type: statblock
name: Force of Earth
level: 3
roles:
  - Elite Brute
ancestry:
  - Elemental
ev: "20"
stamina: "132"
speed: 5
movement: Burrow
size: "2"
stability: 2
free_strike: 6
might: 2
agility: -1
reason: 0
intuition: 1
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Slam Into Dirt
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
      - roll: Power Roll + 2
        tier1: 8 damage
        tier2: 12 damage; M < 1 restrained (save ends)
        tier3: 15 damage; M < 2 restrained (save ends)
      - name: Effect
        effect: The target's space is difficult terrain.
  - type: feature
    feature_type: ability
    name: Convocation of Quartz
    icon: 🏹
    keywords:
      - Magic
      - Ranged
    usage: Maneuver
    distance: Ranged 5
    target: Self or one elemental
    effects:
      - name: Effect
        effect: Until the start of the force's next turn, any melee strike made against
          the target takes a bane if it doesn't already have a bane or double
          bane.
      - cost: 3 Malice
        effect: Until the end of the encounter, the target grows a carapace of stone.
          They have a +3 bonus to stability and gain 15 temporary Stamina.
  - type: feature
    feature_type: ability
    name: Break Armor
    icon: ❗️
    cost: 1 Malice
    keywords:
      - "-"
    usage: Triggered action
    distance: Self
    target: Self
    trigger: The force takes damage.
    effects:
      - name: Effect
        effect: The force halves the damage, and has damage weakness 3 and a +3 bonus to
          speed until the end of the encounter. This damage weakness increases
          by 3 each time the force uses this ability in the same encounter.
  - type: feature
    feature_type: trait
    name: Fickle and Free
    icon: ⭐️
    effects:
      - effect: The force can't be restrained, slowed, or knocked prone, and they ignore
          difficult terrain.
  - type: feature
    feature_type: trait
    name: Primordial Strength
    icon: ⭐️
    effects:
      - effect: The force's strikes gain a +6 damage bonus against objects.
  - type: feature
    feature_type: trait
    name: Stone Swim
    icon: ⭐️
    effects:
      - effect: The force can burrow through stone, but can't drag other creatures
          underground when they do so.
~~~