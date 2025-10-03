---
agility: -1
ancestry:
- Dragon
- Elemental
ev: '96'
file_basename: Crucible Dragon
file_dpath: Monsters/Dragons/Statblocks
free_strike: 7
intuition: 3
item_id: crucible-dragon
item_index: '343'
item_name: Crucible Dragon
level: 6
might: 4
presence: 2
reason: 3
roles:
- Solo
scc:
- mcdm.monsters.v1:monster:crucible-dragon
scdc:
- 1.1.1:2:343
size: '4'
source: mcdm.monsters.v1
speed: 8
stability: 6
stamina: '450'
type: monster
---

~~~ds-statblock
type: statblock
name: Crucible Dragon
level: 6
roles:
  - Solo
ancestry:
  - Dragon
  - Elemental
ev: "96"
stamina: "450"
immunities:
  - Fire 6
speed: 8
size: "4"
stability: 6
free_strike: 7
might: 4
agility: -1
reason: 3
intuition: 3
presence: 2
features:
  - type: feature
    feature_type: trait
    name: Solo Monster
    icon: ☠️
    effects:
      - name: End Effect
        effect: At the end of each of their turns, the dragon can take 10 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
      - name: Solo Turns
        effect: The dragon can take two turns each round. They can't take turns
          consecutively.
  - type: feature
    feature_type: trait
    name: Magnetized Wyrmscale Aura
    icon: ❇️
    effects:
      - effect: The dragon's scales create a 3 aura of magnetism around them that
          affects large masses of metal. Any creature who enters the area for
          the first time in a round or starts their turn there while wearing
          metal or while slagged (see Slag Spew) is pulled up to 2 squares
          toward the dragon. A creature pulled this way who has M < 3 is unable
          to willingly move away from the dragon.
  - type: feature
    feature_type: ability
    name: Slag Spew
    icon: 🔳
    ability_type: Signature Ability
    keywords:
      - Area
      - Magic
    usage: Main action
    distance: 10 x 2 line within 1
    target: Each creature and object in the area
    effects:
      - name: Effect
        effect: Each target makes an Agility test.
        tier1: 13 fire damage; the target is slagged (save ends)
        tier2: 10 fire damage; the target is slagged (save ends)
        tier3: 6 fire damage
      - effect: A slagged target is coated in molten metal and takes 2d6 fire damage at
          the start of each of their turns. If a slagged target has M < 3 they
          are restrained (save ends) whenever they take cold damage.
  - type: feature
    feature_type: ability
    name: Forge Hammer Tail Slam
    icon: 🗡
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 3
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        tier1: 11 damage; M < 2 prone
        tier2: 17 damage; M < 3 prone
        tier3: 20 damage; M < 4 prone
      - name: Effect
        effect: The dragon can make a free strike against each slagged target knocked
          prone this way.
      - cost: 1 Malice
        effect: The strike deals 1d6 cold damage.
  - type: feature
    feature_type: trait
    name: Heat Buffer
    icon: ⭐️
    effects:
      - effect: Once per round while the dragon is flying using their Thermodynamic
          Flight ability, they give off a blast of steam to extend the duration
          of their flight until the end of the next round. Each creature in a 4
          cube within 1 underneath the dragon when they use this ability takes 7
          fire damage.
  - type: feature
    feature_type: ability
    name: Thermodynamic Flight
    icon: ❇️
    cost: 1 Malice
    keywords:
      - Area
    usage: Maneuver
    distance: 2 burst
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: The dragon expels blistering steam, dealing 7 fire damage to each target
          in the area. The dragon then shifts up to their speed vertically and
          can fly until the end of the round.
  - type: feature
    feature_type: ability
    name: Hammer and Anvil
    icon: ❗️
    cost: 1 Malice
    keywords:
      - "-"
    usage: Free triggered action
    distance: Self
    target: Self
    trigger: While flying, the dragon starts their turn or moves.
    effects:
      - name: Effect
        effect: The dragon drops to the ground and uses Forge Hammer Tail Slam, which
          deals an extra 4 damage for each square they descended.
  - type: feature
    feature_type: ability
    name: Polarize Aura
    icon: ❗️
    cost: 1 Malice
    keywords:
      - Area
      - Magic
    usage: Triggered action
    distance: 3 burst
    target: Each creature and object in the area
    trigger: The dragon is targeted by two melee strikes in the current turn.
    effects:
      - name: Special
        effect: The target must be size 2 or smaller.
      - roll: Power Roll + 4
        tier1: Push 5
        tier2: Push 7
        tier3: Push 10, ignoring stability
  - type: feature
    feature_type: ability
    name: Heart of the Forge
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
      - Magic
    usage: "-"
    distance: 6 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        tier1: 4 fire damage; I < 2 frightened (save ends)
        tier2: 6 fire damage; I < 3 frightened (save ends)
        tier3: 8 fire damage; I < 4 frightened (save ends)
  - type: feature
    feature_type: ability
    name: Subdermal Shielding
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - "-"
    usage: "-"
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: Shields embedded under the dragon's scales emerge, and the dragon gains
          damage immunity 6 at the start of each round until the end of the
          encounter. If the dragon takes any damage, they lose this immunity
          until the end of the current round.
  - type: feature
    feature_type: ability
    name: Polarity Chaos
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - "-"
    usage: "-"
    distance: 10 burst
    target: Each creature and object in the area
    effects:
      - name: Effect
        effect: Each target makes a **Might test**.
        tier1: 16 damage; pull 10 or push 10
        tier2: 13 damage; pull 8 or push 8
        tier3: 7 damage; pull 5 or push 5.
  - type: feature
    feature_type: trait
    name: Swordfall
    icon: 🔳
    cost: 3 Malice
    effects:
      - effect: While the dragon is flying, they shape themself into a blade and fall.
          Each creature and object in the dragon's space when they hit the
          ground and in a 6 x 4 line within 1 square of the dragon takes 7
          damage. A creature who takes this damage and has A < 4 takes 4 extra
          damage per square the dragon fell and is restrained (save ends). A
          creature not restrained this way can move into the nearest unoccupied
          space.
  - type: feature
    feature_type: trait
    name: Shower of Blades
    icon: 🔳
    cost: 5 Malice
    effects:
      - effect: The dragon shakes loose a cloud of shattered weapons in a 6 x 4 line
          within 1 square of them. Each creature and object in the area makes an
          **Agility test**.
        tier1: 16 damage; bleeding (save ends)
        tier2: 13 damage; bleeding (EoT)
        tier3: 7 damage
  - type: feature
    feature_type: trait
    name: Solo Action
    icon: ☠️
    cost: 5 Malice
    effects:
      - effect: The dragon takes an additional main action on their turn. They can use
          this feature even if they are dazed.
  - type: feature
    feature_type: trait
    name: Meltdown
    icon: 🌀
    cost: 7 Malice
    effects:
      - effect: The dragon superheats the ground across the encounter map until the end
          of the round. Any enemy who starts their turn on the ground is slagged
          as if affected by the dragon's Slag Spew ability.
~~~