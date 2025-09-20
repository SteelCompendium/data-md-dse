---
agility: 3
ancestry:
- Draconian
- Dragon
- Humanoid
ev: '32'
file_basename: Myxovidan the Sintaker
file_dpath: Monsters/Draconians/Statblocks
free_strike: 7
intuition: 2
item_id: myxovidan-the-sintaker
item_index: '102'
item_name: Myxovidan the Sintaker
level: 6
might: -1
presence: 1
reason: 2
roles:
- Elite Hexer
scc:
- mcdm.monsters.v1:monster:myxovidan-the-sintaker
scdc:
- 1.1.1:2:102
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '140'
type: monster
---

~~~ds-statblock
type: statblock
name: Myxovidan the Sintaker
level: 6
roles:
  - Elite Hexer
ancestry:
  - Draconian
  - Dragon
  - Humanoid
ev: "32"
stamina: "140"
immunities:
  - Corruption 6
speed: 5
movement: Fly
size: 1M
stability: 2
free_strike: 7
might: -1
agility: 3
reason: 2
intuition: 2
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Breaking Palm
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 1
    target: Two enemies
    effects:
      - roll: Power Roll + 3
        tier1: 10 damage; M < 1 weakened (save ends)
        tier2: 15 damage; M < 2 weakened (save ends)
        tier3: 18 corruption damage; M < 3 weakened (save ends)
      - cost: 2 Malice
        effect: Myxovidan regains Stamina equal to half the damage dealt.
  - type: feature
    feature_type: ability
    name: Expunging Exhalation
    icon: ❇️
    keywords:
      - Area
      - Magic
    usage: Main action
    distance: 2 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        tier1: 7 corruption damage; M < 1 the target has corruption weakness 3 (save
          ends)
        tier2: 12 corruption damage; M < 2 the target has corruption weakness 3 (save
          ends)
        tier3: 15 corruption damage; M < 3 the target has corruption weakness 3 (save
          ends)
  - type: feature
    feature_type: ability
    name: Step and Swap
    icon: 🏹
    keywords:
      - Ranged
    usage: Maneuver
    distance: Ranged 3
    target: One ally
    effects:
      - name: Effect
        effect: Myxovidan and the target shift to swap places.
  - type: feature
    feature_type: ability
    name: Anyone Can Do That
    icon: ❗️
    cost: 2 Malice
    keywords:
      - "-"
    usage: Triggered action
    distance: Self
    target: Self
    trigger: An adjacent creature damages Myxovidan with a melee ability.
    effects:
      - name: Effect
        effect: Myxovidan recreates the ability to use it against the triggering
          creature. If the ability has a power roll, Myxovidan uses his highest
          characteristic score for the roll. If Myxovidan gets a higher tier
          outcome than the triggering creature, the Director gains 2 Malice.
  - type: feature
    feature_type: trait
    name: Stench of Death
    icon: ⭐️
    effects:
      - effect: Whenever an enemy regains Stamina while within 5 squares of Myxovidan,
          they regain 3 less Stamina.
~~~