---
agility: -1
ancestry:
- Construct
- Undead
ev: '72'
file_basename: Ashen Hoarder
file_dpath: Monsters/Ashen Hoarder/Statblocks
free_strike: 6
intuition: 0
item_id: ashen-hoarder
item_index: '206'
item_name: Ashen Hoarder
level: 4
might: 4
presence: -5
reason: -2
roles:
- Solo
scc:
- mcdm.monsters.v1:monster:ashen-hoarder
scdc:
- 1.1.1:2:206
size: '3'
source: mcdm.monsters.v1
speed: 8
stability: 3
stamina: '350'
type: monster
---

~~~ds-statblock
type: statblock
name: Ashen Hoarder
level: 4
roles:
  - Solo
ancestry:
  - Construct
  - Undead
ev: "72"
stamina: "350"
weaknesses:
  - Holy 5
speed: 8
movement: Burrow
size: "3"
stability: 3
free_strike: 6
might: 4
agility: -1
reason: -2
intuition: 0
presence: -5
features:
  - type: feature
    feature_type: trait
    name: Solo Monster
    icon: ☠️
    effects:
      - name: End Effect
        effect: At the end of each of their turns, the ashen hoarder can take 10 damage
          to end one effect on them that can be ended by a saving throw. This
          damage can't be reduced in any way.
      - name: Solo Turns
        effect: The ashen hoarder can take two turns each round. They can't take turns
          consecutively.
  - type: feature
    feature_type: ability
    name: Claw and Blade
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
      - roll: Power Roll + 4
        tier1: 10 damage; if one target has M < 2 they are bleeding (save ends); if the
          other target has A < 2 they are grabbed
        tier2: 15 damage; if one target has M < 3 they are bleeding (save ends); if the
          other target has A < 3 they are grabbed
        tier3: 18 damage; M < 4 bleeding (save ends); A < 2 grabbed
      - name: Effect
        effect: The ashen hoarder can have up to two size 1 creatures grabbed at a time.
          | |
  - type: feature
    feature_type: ability
    name: Corpse Bomb
    icon: 🔳
    keywords:
      - Area
      - Magic
      - Ranged
    usage: Main Action
    distance: 4 cube within 20
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        tier1: 4 damage; A < 2 weakened (save ends)
        tier2: 8 damage; A < 3 weakened (save ends)
        tier3: 11 damage; A < 4 weakened (save ends)
      - cost: 2 Malice
        effect: Any enemy weakened this way is instead slowed and weakened (save ends).
      - cost: 3 Malice
        effect: The ashen hoarder targets a second 4 cube within distance.
  - type: feature
    feature_type: ability
    name: Impale
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
      - Weapon
    usage: Main action
    distance: 4 x 1 line within 1
    target: Each creature in the area
    effects:
      - roll: Power Roll + 4
        tier1: 6 corruption damage; M < 2 the target is impaled (save ends)
        tier2: 11 corruption damage; M < 3 the target is impaled (save ends)
        tier3: 14 corruption damage; M < 4 the target is impaled (save ends)
      - name: Effect
        effect: An impaled creature is restrained and bleeding, and moves with the ashen
          hoarder. The ashen hoarder can have three creatures impaled with this
          ability at a time.
  - type: feature
    feature_type: ability
    name: Bone Dozer
    icon: 👤
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The ashen hoarder moves up to twice their speed in a straight line. Each
          creature or object in the path of this movement is either pushed into
          the nearest unoccupied space outside the path, or if they have M < 3
          is pushed forward until the movement ends. Any creature who is force
          moved forward into an obstacle is dazed (save ends).
  - type: feature
    feature_type: ability
    name: Armor of Corpses
    icon: ❗️
    cost: 2 Malice
    keywords:
      - "-"
    usage: Triggered action
    distance: Self
    target: Self
    trigger: The ashen hoarder takes damage.
    effects:
      - name: Effect
        effect: The ashen hoarder halves the damage. If the ashen hoarder has one or
          more creatures impaled, the Malice cost of this feature is reduced by
          1 and one impaled creature takes the other half of the damage.
  - type: feature
    feature_type: trait
    name: Bladed Body
    icon: ⭐️
    effects:
      - effect: An adjacent enemy who grabs the ashen hoarder or uses a melee ability
          against them takes 3 damage.
  - type: feature
    feature_type: trait
    name: Soul Singularity
    icon: ⭐️
    effects:
      - effect: When the ashen hoarder is reduced to 0 Stamina, they explode in a
          swirling singularity of bone shards and soul energy. Each creature
          within 5 squares of the ashen hoarder who has M < 3 takes 11
          corruption damage. A creature killed by this damage has their soul
          sucked into the vortex and lost somewhere in the Abyssal Wasteland,
          and can't be brought back to life until their soul is recovered.
  - type: feature
    feature_type: ability
    name: Skeletal Eruption
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
      - Weapon
    usage: "-"
    distance: 8 x 3 line within 1
    target: Each creature and object in the area
    effects:
      - roll: Power Roll + 4
        tier1: 6 damage, vertical push 2
        tier2: 11 damage, vertical push 2
        tier3: 14 damage, vertical push 3
      - name: Effect
        effect: Each target is force moved straight up, then falls. A target who would
          normally land prone after falling is instead restrained (save ends).
  - type: feature
    feature_type: ability
    name: Mobile Mine Field
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - Area
      - Ranged
    usage: "-"
    distance: 10 cube within 20
    target: Special
    effects:
      - name: Effect
        effect: The ashen hoarder sprays out six size 1M zombie mines that appear in
          unoccupied squares within distance. Any enemy who moves adjacent to a
          zombie mine for the first time in a round or starts their turn there
          causes the mine to explode, dealing 4 corruption damage to each
          creature adjacent to the mine. Any other zombie mines adjacent to the
          exploding mine also explode. At the start of each of the ashen
          hoarder's turns, each unexploded zombie mine can be moved up to 2
          squares.
  - type: feature
    feature_type: ability
    name: Ossuary Assault
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: "-"
    distance: Self; see below
    target: Self
    effects:
      - name: Effect
        effect: The ashen hoarder moves up to their speed and uses Claw and Blade with a
          double edge against one target. On a tier 3 outcome, the ashen hoarder
          can use Impale without spending Malice.
~~~