---
agility: -1
ancestry:
- Animal
- Orc
ev: '20'
file_basename: Scyza
file_dpath: Monsters/Orcs/Statblocks
free_strike: 5
intuition: 0
item_id: scyza
item_index: '131'
item_name: Scyza
level: 3
might: 2
presence: -1
reason: -4
roles:
- Elite Mount
scc:
- mcdm.monsters.v1:monster:scyza
scdc:
- 1.1.1:2:131
size: '4'
source: mcdm.monsters.v1
speed: 6
stability: 3
stamina: '100'
type: monster
---

~~~ds-statblock
type: statblock
name: Scyza
level: 3
roles:
  - Elite Mount
ancestry:
  - Animal
  - Orc
ev: "20"
stamina: "100"
speed: 6
size: "4"
stability: 3
free_strike: 5
might: 2
agility: -1
reason: -4
intuition: 0
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Clawed Kick
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
        tier1: 7 damage
        tier2: 11 damage; prone
        tier3: 14 damage; prone
      - name: Effect
        effect: The scyza roars, and if the target has I < 2, they are frightened (save
          ends).
  - type: feature
    feature_type: ability
    name: Whiptail
    icon: 🗡
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 3
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 8 damage
        tier2: 13 damage; prone
        tier3: 16 damage; A < 2 bleeding (save ends)
      - name: Effect
        effect: Against a target on top of the scyza, this ability gains an edge, and
          the target is pushed into an unoccupied adjacent square and knocked
          prone.
  - type: feature
    feature_type: ability
    name: Crestfall
    icon: 🔳
    cost: 2 Malice
    keywords:
      - Area
      - Ranged
      - Weapon
    usage: Main action
    distance: 3 cube within 2
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        tier1: 4 damage, 1 sonic damage; R < 0 dazed (save ends)
        tier2: 7 damage, 2 sonic damage; R < 1 dazed (save ends)
        tier3: 9 damage, 3 sonic damage; R < 2 dazed (save ends)
  - type: feature
    feature_type: ability
    name: Sandstorm
    icon: ❇️
    cost: 3 Malice
    keywords:
      - Area
    usage: Maneuver
    distance: 3 burst
    target: Special
    effects:
      - name: Effect
        effect: The scyza kicks up a sandstorm, granting concealment to themself and any
          ally in the area until the end of the scyza's next turn. Each enemy in
          the area makes an Intuition test.
        tier1: 10 damage; prone; slowed (EoT)
        tier2: 7 damage; slowed (EoT)
        tier3: 4 damage
  - type: feature
    feature_type: ability
    name: Brace and Break
    icon: ❗️
    keywords:
      - "-"
    usage: Triggered action
    distance: Self
    target: Self
    trigger: The scyza or an ally riding the scyza is targeted by an ability.
    effects:
      - name: Effect
        effect: Any damage dealt by the triggering ability is halved. If the creature or
          object who used the ability is within 3 squares of the scyza, the
          scyza can make a free strike against them.
  - type: feature
    feature_type: trait
    name: Terrible Beast
    icon: ⭐️
    effects:
      - effect: The scyza deals an extra 6 damage with abilities used against objects.
  - type: feature
    feature_type: trait
    name: War Harness
    icon: ⭐️
    effects:
      - effect: While riding the scyza, three size 1 allies can occupy the same space.
~~~