---
agility: 2
ancestry:
- Beast
- Chimera
ev: '60'
file_basename: Chimera
file_dpath: Monsters/Chimera/Statblocks
free_strike: 6
intuition: 1
item_id: chimera
item_index: '01'
item_name: Chimera
level: 3
might: 3
presence: 0
reason: -2
roles:
- Solo
scc:
- mcdm.monsters.v1:monster:chimera
scdc:
- 1.1.1:2:01
size: '2'
source: mcdm.monsters.v1
speed: 10
stability: 1
stamina: '300'
type: monster
---

~~~ds-statblock
type: statblock
name: Chimera
level: 3
roles:
  - Solo
ancestry:
  - Beast
  - Chimera
ev: "60"
stamina: "300"
immunities:
  - Fire 6
speed: 10
movement: Fly
size: "2"
stability: 1
free_strike: 6
might: 3
agility: 2
reason: -2
intuition: 1
presence: 0
features:
  - type: feature
    feature_type: trait
    name: Solo Monster
    icon: ☠️
    effects:
      - name: End Effect
        effect: At the end of each of their turns, the chimera can take 5 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
      - name: Solo Turns
        effect: The chimera can take two turns each round. They can't take turns
          consecutively.
  - type: feature
    feature_type: trait
    name: Volant
    icon: ⭐️
    effects:
      - effect: When the chimera makes a creature winded or reduces them to 0 Stamina,
          they can move their speed toward an enemy.
  - type: feature
    feature_type: ability
    name: Bite
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
      - roll: Power Roll + 3
        tier1: 9 damage
        tier2: 13 damage
        tier3: 16 damage
      - name: Effect
        effect: This strike deals an extra 3 damage if it gains an edge or has a double
          edge.
  - type: feature
    feature_type: ability
    name: Dragon's Eruption
    icon: 🔳
    cost: 5 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    usage: Main action
    distance: 3 cube within 10
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        tier1: 3 fire damage; A < 1 3 fire damage
        tier2: 5 fire damage; A < 2 5 fire damage
        tier3: 7 fire damage; A < 3 7 fire damage
  - type: feature
    feature_type: ability
    name: Roar
    icon: ❇️
    cost: 5 Malice
    keywords:
      - Area
      - Magic
    usage: Main action
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        tier1: 4 psychic damage
        tier2: 8 psychic damage; I < 2 frightened (save ends)
        tier3: 10 psychic damage; I < 3 frightened (save ends)
  - type: feature
    feature_type: ability
    name: Lion's Toss
    icon: 🗡
    keywords:
      - Melee
      - Weapon
    usage: Maneuver
    distance: Melee 2
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        tier1: Vertical push 2
        tier2: Vertical push 3
        tier3: Vertical push 5
  - type: feature
    feature_type: ability
    name: Ram's Defiance
    icon: ❗️
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Triggered action
    distance: Melee 2
    target: The triggering creature
    trigger: A creature makes a strike against the chimera and obtains a tier 1 outcome.
    effects:
      - name: Effect
        effect: The chimera shifts up to 5 squares. If they end this shift within
          distance of the target, make a power roll.
      - effect: "**Power Roll + 3**"
        tier1: 6 damage; M < 1 slowed (save ends)
        tier2: 8 damage; prone; M < 2 slowed (save ends)
        tier3: 10 damage; prone; M < 3 slowed (save ends)
  - type: feature
    feature_type: ability
    name: Overture of Destruction
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
    usage: "-"
    distance: 1 burst
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: The chimera can use Bite and Lion's Toss against each target.
  - type: feature
    feature_type: ability
    name: Fire Solo
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - "-"
    usage: "-"
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The chimera uses Dragon's Eruption and Roar without spending Malice.
  - type: feature
    feature_type: ability
    name: Chorus of Destruction
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - "-"
    usage: "-"
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The chimera uses Roar, then shifts up to their speed and can make a free
          strike against each enemy who comes adjacent to them during the shift.
          When the chimera ends this shift, they use Dragon's Eruption. The use
          of these abilities as part of this villain action costs no Malice.
~~~