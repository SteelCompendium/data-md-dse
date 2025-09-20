---
agility: 0
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '4'
file_basename: War Dog Subcommander
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 2
intuition: 0
item_id: war-dog-subcommander
item_index: '370'
item_name: War Dog Subcommander
level: 2
might: 2
presence: 1
reason: 0
roles:
- Horde Support
scc:
- mcdm.monsters.v1:monster:war-dog-subcommander
scdc:
- 1.1.1:2:370
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '20'
type: monster
---

~~~ds-statblock
type: statblock
name: War Dog Subcommander
level: 2
roles:
  - Horde Support
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "4"
stamina: "20"
speed: 5
size: 1M
stability: 0
free_strike: 2
might: 2
agility: 0
reason: 0
intuition: 0
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Command Saber
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        tier1: 4 damage
        tier2: 5 damage
        tier3: 7 damage
      - name: Effect
        effect: One ally within 5 squares of the subcommander can make a free strike
          against the target.
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
    feature_type: trait
    name: The Iron Saint Does Not Recognize Retreat
    icon: ⭐️
    effects:
      - effect: Each ally within 5 squares of the subcommander gains a +3 bonus to
          stability.
  - type: feature
    feature_type: trait
    name: Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When the subcommander is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 1d6 damage to each adjacent enemy and object.
~~~