---
agility: 1
ancestry:
- Giant
- Troll
ev: '28'
file_basename: Troll Butcher
file_dpath: Monsters/Trolls/Statblocks
free_strike: 6
intuition: 0
item_id: troll-butcher
item_index: '407'
item_name: Troll Butcher
level: 5
might: 3
presence: 0
reason: 1
roles:
- Elite Hexer
scc:
- mcdm.monsters.v1:monster:troll-butcher
scdc:
- 1.1.1:2:407
size: '2'
source: mcdm.monsters.v1
speed: 8
stability: 2
stamina: '120'
type: monster
---

~~~ds-statblock
type: statblock
name: Troll Butcher
level: 5
roles:
  - Elite Hexer
ancestry:
  - Giant
  - Troll
ev: "28"
stamina: "120"
weaknesses:
  - Acid 5
  - fire
speed: 8
size: "2"
stability: 2
free_strike: 6
might: 3
agility: 1
reason: 1
intuition: 0
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Savoring Bite
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
      - roll: Power Roll + 3
        tier1: 9 damage; M < 1 bleeding (save ends)
        tier2: 14 damage; M < 2 bleeding (save ends)
        tier3: 17 damage; M < 3 bleeding (save ends)
      - cost: 1 Malice
        effect: The butcher regains Stamina equal to the damage dealt.
  - type: feature
    feature_type: ability
    name: Rotten Scraps
    icon: 🔳
    keywords:
      - Area
      - Ranged
    usage: Main action
    distance: 3 cube within 10
    target: Each creature in the area
    effects:
      - roll: Power Roll + 3
        tier1: 5 poison damage; M < 1 weakened (save ends)
        tier2: 9 poison damage; M < 2 weakened (save ends)
        tier3: 11 poison damage; M < 3 weakened (save ends)
      - name: Effect
        effect: Each troll in the area ignores the damage and instead regains 3 Stamina.
  - type: feature
    feature_type: ability
    name: Gourmet Flesh
    icon: 👤
    cost: 2 Malice
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: "The butcher enhances their next use of Savoring Bite, changing the
          damage type and condition imposed to one of the following pairs:
          corruption damage and dazed, acid damage and restrained, or lightning
          damage and frightened."
  - type: feature
    feature_type: ability
    name: Acquired Taste
    icon: ❗️
    keywords:
      - Melee
    usage: Triggered action
    distance: Melee 1
    target: The triggering creature
    trigger: A creature within distance deals damage to the butcher with an ability
      that gains an edge, has a double edge, or uses a surge.
    effects:
      - name: Effect
        effect: The butcher makes a free strike against the target. Until the end of
          their next turn, the butcher gains an edge on power rolls and deals an
          extra 3 damage with strikes.
  - type: feature
    feature_type: trait
    name: Bloody Feast
    icon: ⭐️
    effects:
      - effect: Each ally within 5 squares of the butcher gains an edge on power rolls
          against any enemy affected by a condition.
  - type: feature
    feature_type: trait
    name: Relentless Hunger
    icon: ⭐️
    effects:
      - effect: The butcher dies only if they are reduced to 0 Stamina by acid or fire
          damage, if they end their turn with 0 Stamina, or if they take acid or
          fire damage while at 0 Stamina.
~~~