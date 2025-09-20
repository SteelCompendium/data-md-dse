---
agility: 2
ancestry:
- Humanoid
- Radenwight
ev: '12'
file_basename: Radenwight Maestro
file_dpath: Monsters/Radenwights/Statblocks
free_strike: 4
intuition: 0
item_id: radenwight-maestro
item_index: '151'
item_name: Radenwight Maestro
level: 1
might: -2
presence: 3
reason: 0
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:radenwight-maestro
scdc:
- 1.1.1:2:151
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '80'
type: monster
---

~~~ds-statblock
type: statblock
name: Radenwight Maestro
level: 1
roles:
  - Leader
ancestry:
  - Humanoid
  - Radenwight
ev: "12"
stamina: "80"
speed: 5
movement: Climb
size: 1S
stability: 1
free_strike: 4
might: -2
agility: 2
reason: 0
intuition: 0
presence: 3
features:
  - type: feature
    feature_type: ability
    name: Cacophony
    icon: ❇️
    ability_type: Signature Ability
    keywords:
      - Area
      - Magic
    usage: Main action
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        tier1: 3 sonic damage; slide 1, the maestro can shift 1 square
        tier2: 6 sonic damage; slide 3, the maestro shifts up to 3 squares
        tier3: 8 sonic damage; slide 5, the maestro shifts up to 5 squares
      - name: Effect
        effect: Each ally within distance can use Ready Rodent as a free triggered
          action once before the end of the round.
  - type: feature
    feature_type: ability
    name: Tempo Changer
    icon: 🏹
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Maneuver
    distance: Ranged 10
    target: Two enemies
    effects:
      - roll: Power Roll + 3
        tier1: P < 1 slowed (save ends)
        tier2: P < 2 slowed (save ends)
        tier3: P < 3 slowed (save ends)
      - cost: 3 Malice
        effect: Each ally within 3 squares of any target has a +2 bonus to speed until
          the end of their next turn.
  - type: feature
    feature_type: ability
    name: Ever-Ready Rodent
    icon: ❗️
    cost: 2 Malice
    keywords:
      - Magic
      - Ranged
    usage: Free triggered action
    distance: Ranged 5
    target: The triggering creature
    trigger: A creature within distance deals damage to an ally or takes damage from
      an ally.
    effects:
      - name: Effect
        effect: The maestro makes a free strike against the target.
  - type: feature
    feature_type: trait
    name: End Effect
    icon: ⭐️
    effects:
      - effect: At the end of each of their turns, the maestro can take 5 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
  - type: feature
    feature_type: ability
    name: Overture
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
    usage: "-"
    distance: 10 burst
    target: Each ally in the area
    effects:
      - name: Effect
        effect: Each target can shift up to their speed or take the Defend action.
  - type: feature
    feature_type: ability
    name: Solo Act
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - Ranged
    usage: "-"
    distance: Ranged 15
    target: One creature
    effects:
      - name: Effect
        effect: Until the end of their next turn, the target halves any damage they
          take, gains a +4 damage bonus to strikes, and has their speed doubled.
  - type: feature
    feature_type: ability
    name: Rondo of Rat
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Area
    usage: "-"
    distance: 10 burst
    target: Each dead ally in the area
    effects:
      - name: Effect
        effect: Each target stands, makes a free strike, then falls dead again. Any ally
          of the targets can use Ready Rodent as a free triggered action once in
          conjunction with these free strikes.
~~~