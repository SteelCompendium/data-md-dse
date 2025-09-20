---
agility: 4
ancestry:
- Humanoid
- Rival
ev: '40'
file_basename: Rival Shadow
file_dpath: Monsters/Rivals/3rd Echelon/Statblocks
free_strike: 9
intuition: 0
item_id: rival-shadow
item_index: '27'
item_name: Rival Shadow
level: 8
might: 0
presence: 3
reason: 2
roles:
- Elite Ambusher
scc:
- mcdm.monsters.v1:monster:rival-shadow
scdc:
- 1.1.1:2:27
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 1
stamina: '200'
type: monster
---

~~~ds-statblock
type: statblock
name: Rival Shadow
level: 8
roles:
  - Elite Ambusher
ancestry:
  - Humanoid
  - Rival
ev: "40"
stamina: "200"
speed: 7
size: 1M
stability: 1
free_strike: 9
might: 0
agility: 4
reason: 2
intuition: 0
presence: 3
features:
  - type: feature
    feature_type: ability
    name: Assail and Serrate
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
      - roll: Power Roll + 4
        tier1: 13 damage; A < 2 bleeding (save ends)
        tier2: 18 damage; A < 3 bleeding (save ends)
        tier3: 22 damage; A < 4 bleeding and weakened (save ends)
      - cost: 1 Malice
        effect: The shadow can teleport up to 7 squares, then can attempt to hide.
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
        effect: The shadow coats their weapon with poison. They have a double edge on
          their next strike, and any potency for that strike increases by 2.
  - type: feature
    feature_type: trait
    name: Exploit Weakness
    icon: ⭐️
    effects:
      - effect: The shadow deals an extra 9 damage to any target affected by a
          condition.
  - type: feature
    feature_type: trait
    name: Rivalry
    icon: ⭐️
    effects:
      - effect: At the start of an encounter, the shadow chooses one creature within
          their line of effect. Both the shadow and the creature can add a d3
          roll to power rolls they make against each other.
~~~