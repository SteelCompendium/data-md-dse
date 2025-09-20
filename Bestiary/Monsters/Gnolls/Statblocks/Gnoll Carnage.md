---
agility: 3
ancestry:
- Abyssal
- Gnoll
ev: '16'
file_basename: Gnoll Carnage
file_dpath: Monsters/Gnolls/Statblocks
free_strike: 5
intuition: 0
item_id: gnoll-carnage
item_index: '39'
item_name: Gnoll Carnage
level: 2
might: 3
presence: 3
reason: 0
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:gnoll-carnage
scdc:
- 1.1.1:2:39
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '100'
type: monster
---

~~~ds-statblock
type: statblock
name: Gnoll Carnage
level: 2
roles:
  - Leader
ancestry:
  - Abyssal
  - Gnoll
ev: "16"
stamina: "100"
speed: 5
size: 1M
stability: 1
free_strike: 5
might: 3
agility: 3
reason: 0
intuition: 0
presence: 3
features:
  - type: feature
    feature_type: ability
    name: Shrapnel Whip
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
        tier1: 8 damage; A < 1 bleeding (save ends)
        tier2: 11 damage; A < 2 bleeding (save ends)
        tier3: 14 damage; A < 3 bleeding and dazed (save ends)
      - name: Effect
        effect: An ally targeted by this ability ignores the damage and can make a free
          strike.
  - type: feature
    feature_type: ability
    name: Carnage's Cackletongue
    icon: ❇️
    cost: 4 Malice
    keywords:
      - Area
    usage: Maneuver
    distance: 5 burst
    target: Self and each ally in the area
    effects:
      - name: Effect
        effect: Each target deals an extra 3 damage with their next strike until the
          start of the carnage's next turn. If any target hasn't used their own
          Cackletongue maneuver on this turn, they can use it immediately at no
          cost.
  - type: feature
    feature_type: trait
    name: Death Rampage
    icon: ⭐️
    effects:
      - effect: Whenever a non-minion ally within 5 squares of the carnage is reduced to
          0 Stamina, the carnage can move up to their speed, then can either
          make a melee free strike against two creatures or use Shrapnel Whip
          against one creature.
  - type: feature
    feature_type: trait
    name: End Effect
    icon: ⭐️
    effects:
      - effect: At the end of each of their turns, the carnage can take 5 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
  - type: feature
    feature_type: trait
    name: Endless Hunger
    icon: ⭐️
    effects:
      - effect: If the carnage is reduced to 0 Stamina while there are still gnolls on
          the encounter map, one gnoll on the map is transformed into a gnoll
          carnage, keeping their current Stamina.
  - type: feature
    feature_type: ability
    name: Call Up From the Abyss
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Magic
      - Ranged
    usage: "-"
    distance: Ranged 10
    target: Special
    effects:
      - name: Effect
        effect: The carnage summons four abyssal hyenas into unoccupied spaces within
          distance.
  - type: feature
    feature_type: ability
    name: Edacity
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - Area
    usage: "-"
    distance: 10 burst
    target: Self and three allies
    effects:
      - name: Effect
        effect: Each target moves up to their speed and can make a free strike. Any
          creature damaged by one of these free strikes who has M < 2 is knocked
          prone.
  - type: feature
    feature_type: ability
    name: Deepest Wounds
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Area
      - Magic
    usage: "-"
    distance: 5 burst
    target: Each winded enemy in the area
    effects:
      - name: Effect
        effect: The carnage's eyes and all exposed blood within distance glow bright
          red. Each target makes a **Presence test**.
        tier1: The target can't regain Stamina until the end of the encounter.
        tier2: The target can't regain Stamina (save ends).
        tier3: No effect
      - name: Effect
        effect: Until the end of the encounter, all gnolls have a double edge on power
          rolls that target a winded enemy.
~~~