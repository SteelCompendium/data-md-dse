---
agility: 1
ancestry:
- Humanoid
- Lizardfolk
ev: '6'
file_basename: Lizardfolk Scaletooth
file_dpath: Monsters/Lizardfolks/Statblocks
free_strike: 4
intuition: 0
item_id: lizardfolk-scaletooth
item_index: '52'
item_name: Lizardfolk Scaletooth
level: 1
might: 2
presence: 0
reason: 0
roles:
- Platoon Brute
scc:
- mcdm.monsters.v1:monster:lizardfolk-scaletooth
scdc:
- 1.1.1:2:52
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '46'
type: monster
---

~~~ds-statblock
type: statblock
name: Lizardfolk Scaletooth
level: 1
roles:
  - Platoon Brute
ancestry:
  - Humanoid
  - Lizardfolk
ev: "6"
stamina: "46"
speed: 5
movement: Swim
size: 1M
stability: 0
free_strike: 4
might: 2
agility: 1
reason: 0
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Razor Bite
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
        tier1: 6 damage
        tier2: 9 damage
        tier3: 12 damage; A < 2 bleeding (save ends)
      - name: Effect
        effect: If the scaletooth has the target grabbed, the potency of this ability
          increases by 1.
  - type: feature
    feature_type: ability
    name: Tail Whip
    icon: 🗡
    cost: 2 Malice
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        tier1: 5 damage; slide 1
        tier2: 8 damage; slide 2; M < 1 grabbed if within 2 squares of the scaletooth
        tier3: 10 damage; slide 3; M < 2 grabbed if within 2 squares of the scaletooth
  - type: feature
    feature_type: trait
    name: Reptilian Escape
    icon: ⭐️
    effects:
      - effect: While the scaletooth has a tail, whenever they are grabbed, prone,
          slowed, or weakened, they can lose their tail to immediately end that
          condition, then shift up to 2 squares.
~~~