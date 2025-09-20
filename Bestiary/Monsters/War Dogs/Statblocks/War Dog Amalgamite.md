---
agility: 0
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '4'
file_basename: War Dog Amalgamite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 3
intuition: 0
item_id: war-dog-amalgamite
item_index: '380'
item_name: War Dog Amalgamite
level: 2
might: 2
presence: 0
reason: 0
roles:
- Horde Brute
scc:
- mcdm.monsters.v1:monster:war-dog-amalgamite
scdc:
- 1.1.1:2:380
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '25'
type: monster
---

~~~ds-statblock
type: statblock
name: War Dog Amalgamite
level: 2
roles:
  - Horde Brute
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "4"
stamina: "25"
speed: 5
size: "2"
stability: 2
free_strike: 3
might: 2
agility: 0
reason: 0
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Several Arms
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
        tier1: 4 damage
        tier2: 5 damage; A < 1 grabbed
        tier3: 6 damage; A < 2 grabbed
      - name: Effect
        effect: The amalgamite can have up to four targets grabbed at once.
      - cost: 3 Malice
        effect: The amalgamite deals 3 damage to each creature grabbed this way or who
          they already have grabbed, and regains Stamina equal to the damage
          dealt.
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
    name: Loyalty Collar
    icon: ⭐️
    effects:
      - effect: When the amalgamite is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 1d6 damage to each adjacent enemy and object.
~~~