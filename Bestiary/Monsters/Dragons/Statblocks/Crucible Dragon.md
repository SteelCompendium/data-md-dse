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
item_index: '345'
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
- 1.1.1:2:345
size: '4'
source: mcdm.monsters.v1
speed: 8
stability: 6
stamina: '450'
type: monster
---

~~~ds-statblock
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
traits:
  - name: Solo Monster
    effects:
      - effect: At the end of each of their turns, the dragon can take 10 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
        name: End Effect
      - effect: The dragon can take two turns each round. They can't take turns
          consecutively.
        name: Solo Turns
  - name: Magnetized Wyrmscale Aura
    effects:
      - effect: The dragon's scales create a 3 aura of magnetism around them that
          affects large masses of metal. Any creature who enters the area for
          the first time in a round or starts their turn there while wearing
          metal or while slagged (see Slag Spew) is pulled up to 2 squares
          toward the dragon. A creature pulled this way who has M < 3 is unable
          to willingly move away from the dragon.
  - name: Heat Buffer
    effects:
      - effect: Once per round while the dragon is flying using their Thermodynamic
          Flight ability, they give off a blast of steam to extend the duration
          of their flight until the end of the next round. Each creature in a 4
          cube within 1 underneath the dragon when they use this ability takes 7
          fire damage.
  - name: Swordfall
    effects:
      - effect: While the dragon is flying, they shape themself into a blade and fall.
          Each creature and object in the dragon's space when they hit the
          ground and in a 6 x 4 line within 1 square of the dragon takes 7
          damage. A creature who takes this damage and has A < 4 takes 4 extra
          damage per square the dragon fell and is restrained (save ends). A
          creature not restrained this way can move into the nearest unoccupied
          space.
  - name: Shower of Blades
    effects:
      - effect: The dragon shakes loose a cloud of shattered weapons in a 6 x 4 line
          within 1 square of them. Each creature and object in the area makes an
          **Agility test**.
        t1: 16 damage; bleeding (save ends)
        t2: 13 damage; bleeding (EoT)
        t3: 7 damage
  - name: Solo Action
    effects:
      - effect: The dragon takes an additional main action on their turn. They can use
          this feature even if they are dazed.
  - name: Meltdown
    effects:
      - effect: The dragon superheats the ground across the encounter map until the end
          of the round. Any enemy who starts their turn on the ground is slagged
          as if affected by the dragon's Slag Spew ability.
abilities:
  - name: Slag Spew
    icon: 🔳
    cost: Signature Ability
    keywords:
      - Area
      - Magic
    type: Main action
    distance: 10 x 2 line within 1
    target: Each creature and object in the area
    effects:
      - name: Effect
        effect: Each target makes an Agility test.
        t1: 13 fire damage; the target is slagged (save ends)
        t2: 10 fire damage; the target is slagged (save ends)
        t3: 6 fire damage
      - effect: A slagged target is coated in molten metal and takes 2d6 fire damage at
          the start of each of their turns. If a slagged target has M < 3 they
          are restrained (save ends) whenever they take cold damage.
  - name: Forge Hammer Tail Slam
    icon: 🗡
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 3
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        t1: 11 damage; M < 2 prone
        t2: 17 damage; M < 3 prone
        t3: 20 damage; M < 4 prone
      - effect: The dragon can make a free strike against each slagged target knocked
          prone this way.
        name: Effect
      - effect: The strike deals 1d6 cold damage.
        cost: 1 Malice
  - name: Thermodynamic Flight
    icon: ❇️
    cost: 1 Malice
    keywords:
      - Area
    type: Maneuver
    distance: 2 burst
    target: Each enemy in the area
    effects:
      - effect: The dragon expels blistering steam, dealing 7 fire damage to each target
          in the area. The dragon then shifts up to their speed vertically and
          can fly until the end of the round.
        name: Effect
  - name: Hammer and Anvil
    icon: ❗️
    cost: 1 Malice
    keywords:
      - "-"
    type: Free triggered action
    distance: Self
    target: Self
    trigger: While flying, the dragon starts their turn or moves.
    effects:
      - effect: The dragon drops to the ground and uses Forge Hammer Tail Slam, which
          deals an extra 4 damage for each square they descended.
        name: Effect
  - name: Polarize Aura
    icon: ❗️
    cost: 1 Malice
    keywords:
      - Area
      - Magic
    type: Triggered action
    distance: 3 burst
    target: Each creature and object in the area
    trigger: The dragon is targeted by two melee strikes in the current turn.
    effects:
      - name: Special
        effect: The target must be size 2 or smaller.
      - roll: Power Roll + 4
        t1: Push 5
        t2: Push 7
        t3: Push 10, ignoring stability
  - name: Heart of the Forge
    icon: ☠️
    cost: Villain Action 1
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 6 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        t1: 4 fire damage; I < 2 frightened (save ends)
        t2: 6 fire damage; I < 3 frightened (save ends)
        t3: 8 fire damage; I < 4 frightened (save ends)
  - name: Subdermal Shielding
    icon: ☠️
    cost: Villain Action 2
    keywords:
      - "-"
    type: "-"
    distance: Self
    target: Self
    effects:
      - effect: Shields embedded under the dragon's scales emerge, and the dragon gains
          damage immunity 6 at the start of each round until the end of the
          encounter. If the dragon takes any damage, they lose this immunity
          until the end of the current round.
        name: Effect
  - name: Polarity Chaos
    icon: ☠️
    cost: Villain Action 3
    keywords:
      - "-"
    type: "-"
    distance: 10 burst
    target: Each creature and object in the area
    effects:
      - name: Effect
        effect: Each target makes a **Might test**.
        t1: 16 damage; pull 10 or push 10
        t2: 13 damage; pull 8 or push 8
        t3: 7 damage; pull 5 or push 5.
~~~