---
agility: 1
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '7'
file_basename: War Dog War Doc
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 3
intuition: 2
item_id: war-dog-war-doc
item_index: '386'
item_name: War Dog War Doc
level: 5
might: 0
presence: 0
reason: 3
roles:
- Horde Support
scc:
- mcdm.monsters.v1:monster:war-dog-war-doc
scdc:
- 1.1.1:2:386
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '35'
type: monster
---

~~~ds-statblock
type: statblock
name: War Dog War Doc
level: 5
roles:
  - Horde Support
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "7"
stamina: "35"
speed: 5
size: 1L
stability: 1
free_strike: 3
might: 0
agility: 1
reason: 3
intuition: 2
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Syringe Crossbow
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 10
    target: One creature
    effects:
      - roll: Power Roll + 3
        tier1: 6 poison damage
        tier2: 8 poison damage
        tier3: 9 poison damage; M < 3 weakened (save ends)
      - name: Effect
        effect: A target enemy is subject to this ability's power roll. A target ally
          instead gains 5 temporary Stamina and can make a free strike.
  - type: feature
    feature_type: ability
    name: Posthumous Promotion
    icon: 🏹
    keywords:
      - Magic
      - Ranged
    usage: Maneuver
    distance: Ranged 10
    target: One war dog
    effects:
      - name: Effect
        effect: If the target has a loyalty collar, they are reduced to 0 Stamina.
  - type: feature
    feature_type: ability
    name: Sanguine Stimulants
    icon: ❗️
    cost: 1 Malice
    keywords:
      - Magic
      - Ranged
    usage: Triggered action
    distance: Ranged 15
    target: Special
    trigger: One ally within distance dies.
    effects:
      - name: Effect
        effect: Each ally adjacent to the dead ally deals an extra 6 damage on their
          next strike.
  - type: feature
    feature_type: trait
    name: Body Bank Branch Manager
    icon: ⭐️
    effects:
      - effect: If the war doc uses the Reconstitute war dog Malice feature, it costs 1
          Malice less. Additionally, allies can treat the living war doc as a
          corpse when using the Reconstitute feature (see Reconstitute).
~~~