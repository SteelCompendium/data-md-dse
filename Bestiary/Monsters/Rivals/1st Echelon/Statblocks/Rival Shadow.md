---
agility: 2
ancestry:
- Humanoid
- Rival
ev: '16'
file_basename: Rival Shadow
file_dpath: Monsters/Rivals/1st Echelon/Statblocks
free_strike: 5
intuition: 0
item_id: rival-shadow
item_index: '13'
item_name: Rival Shadow
level: 2
might: 0
presence: 1
reason: 0
roles:
- Elite Ambusher
scc:
- mcdm.monsters.v1:monster:rival-shadow
scdc:
- 1.1.1:2:13
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 1
stamina: '80'
type: monster
---

~~~ds-statblock
type: statblock
name: Rival Shadow
level: 2
roles:
  - Elite Ambusher
ancestry:
  - Humanoid
  - Rival
ev: "16"
stamina: "80"
speed: 7
size: 1M
stability: 1
free_strike: 5
might: 0
agility: 2
reason: 0
intuition: 0
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Swift Serration
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
        tier1: 7 damage
        tier2: 11 damage
        tier3: 14 damage; A < 2 bleeding (save ends)
      - cost: 1 Malice
        effect: The shadow can teleport up to 5 squares, then can attempt to hide.
  - type: feature
    feature_type: ability
    name: Poison the Blade
    icon: 👤
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The shadow coats their weapon with poison. They gain an edge on their
          next strike, and any potency for that strike increases by 1.
  - type: feature
    feature_type: trait
    name: Exploit Opening
    icon: ⭐️
    effects:
      - effect: The shadow deals an extra 5 damage to any bleeding target.
  - type: feature
    feature_type: trait
    name: Rivalry
    icon: ⭐️
    effects:
      - effect: At the start of an encounter, the shadow chooses one creature within
          their line of effect. Both the shadow and the creature can add a d3
          roll to power rolls they make against each other.
~~~