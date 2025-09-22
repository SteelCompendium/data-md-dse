---
agility: 2
ancestry:
- Accursed
- Humanoid
- Minotaur
ev: '20'
file_basename: Minotaur
file_dpath: Monsters/Minotaurs/Statblocks
free_strike: 5
intuition: 1
item_id: minotaur
item_index: '173'
item_name: Minotaur
level: 3
might: 2
presence: -1
reason: 0
roles:
- Elite Harrier
scc:
- mcdm.monsters.v1:monster:minotaur
scdc:
- 1.1.1:2:173
size: '2'
source: mcdm.monsters.v1
speed: 8
stability: 2
stamina: '100'
type: monster
---

~~~ds-statblock
type: statblock
name: Minotaur
level: 3
roles:
  - Elite Harrier
ancestry:
  - Accursed
  - Humanoid
  - Minotaur
ev: "20"
stamina: "100"
speed: 8
size: "2"
stability: 2
free_strike: 5
might: 2
agility: 2
reason: 0
intuition: 1
presence: -1
features:
  - type: feature
    feature_type: ability
    name: Flail and Blade
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        tier1: 7 damage; push 1
        tier2: 11 damage; push 2
        tier3: 14 damage; push 3
      - name: Effect
        effect: The minotaur shifts up to 3 squares.
  - type: feature
    feature_type: ability
    name: Primal Bay
    icon: 👤
    cost: 3 Malice
    keywords:
      - "-"
    usage: Main action
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: Until the end of their next turn, the minotaur has damage immunity 2 and
          deals an extra 5 damage with strikes. On their next turn, the minotaur
          can use one additional maneuver.
  - type: feature
    feature_type: ability
    name: Goring Horns
    icon: 🗡
    cost: 5 Malice
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    usage: Maneuver
    distance: Melee 2
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 5 damage; I < 0 dazed (save ends)
        tier2: 8 damage; I < 1 dazed (save ends)
        tier3: 9 damage; I < 2 dazed (save ends)
      - name: Effect
        effect: If this ability is used as part of the Charge main action, its potency
          increases by 1.
  - type: feature
    feature_type: ability
    name: Retaliatory Strike
    icon: ❗️
    keywords:
      - Ranged
    usage: Triggered action
    distance: Ranged 8
    target: The triggering creature
    trigger: A creature within distance deals damage to the minotaur.
    effects:
      - name: Effect
        effect: The minotaur uses the Charge main action and either Flail and Blade or
          Goring Horns against the target.
  - type: feature
    feature_type: trait
    name: Minotaur Sense
    icon: ⭐️
    effects:
      - effect: The minotaur can't obtain less than a tier 2 outcome when making tests
          to navigate, search, or seek.
~~~