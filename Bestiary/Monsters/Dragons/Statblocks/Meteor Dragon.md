---
agility: 5
ancestry:
- Dragon
- Elemental
ev: '144'
file_basename: Meteor Dragon
file_dpath: Monsters/Dragons/Statblocks
free_strike: 10
intuition: 3
item_id: meteor-dragon
item_index: '346'
item_name: Meteor Dragon
level: 10
might: 5
presence: 5
reason: 3
roles:
- Solo
scc:
- mcdm.monsters.v1:monster:meteor-dragon
scdc:
- 1.1.1:2:346
size: '3'
source: mcdm.monsters.v1
speed: 15
stability: 6
stamina: '650'
type: monster
---

~~~ds-statblock
type: statblock
name: Meteor Dragon
level: 10
roles:
  - Solo
ancestry:
  - Dragon
  - Elemental
ev: "144"
stamina: "650"
speed: 15
movement: Fly
size: "3"
stability: 6
free_strike: 10
might: 5
agility: 5
reason: 3
intuition: 3
presence: 5
features:
  - type: feature
    feature_type: trait
    name: Solo Monster
    icon: ☠️
    effects:
      - name: End Effect
        effect: At the end of each of their turns, the dragon can take 20 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
      - name: Solo Turns
        effect: The dragon can take two turns each round. They can't take turns
          consecutively.
  - type: feature
    feature_type: trait
    name: Voidshroud Wyrmscale Aura
    icon: ❇️
    effects:
      - effect: The dragon's scales create a 1 aura of void space around them. Any enemy
          who starts their turn in the area takes 10 cold damage and is
          suffocating. Each time the dragon takes damage, the area of the aura
          increases by 1 (to a maximum of 5), and they deal an extra 5 damage
          the next time they use an ability that deals rolled damage.
  - type: feature
    feature_type: ability
    name: Gravity Well
    icon: 🔳
    ability_type: Signature Ability
    keywords:
      - Area
      - Magic
      - Ranged
    usage: Main action
    distance: 4 cube within 10
    target: Each creature and object in the area
    effects:
      - name: Effect
        effect: Each target makes a **Might test**.
        tier1: 20 sonic damage; the target is dragonsealed (save ends)
        tier2: 16 sonic damage; the target is dragonsealed (save ends)
        tier3: 10 sonic damage
      - effect: A dragonsealed target emits a golden aura, and takes 2 damage per square
          moved when falling or when force moved into an obstacle.
  - type: feature
    feature_type: ability
    name: Cosmic Tail Ray
    icon: ⚔️
    keywords:
      - Magic
      - Melee
      - Ranged
      - Strike
    usage: Main action
    distance: Melee 2 or ranged 15
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 5
        tier1: 15 holy damage; A < 4 weakened (save ends)
        tier2: 21 holy damage; A < 5 weakened (save ends)
        tier3: 25 holy damage; A < 6 weakened (save ends)
      - name: Effect
        effect: If a target made weakened this way is already weakened, they are instead
          dazed until the end of their next turn.
  - type: feature
    feature_type: trait
    name: Crescent Claws
    icon: ⭐️
    effects:
      - effect: Once per turn, the dragon chooses a target within 3 squares. The dragon
          can make a free strike against the target, and ignores banes when
          using abilities against the target until the start of their next turn.
  - type: feature
    feature_type: ability
    name: Investiture of Gravity
    icon: ❇️
    cost: 5 Malice
    keywords:
      - Area
      - Magic
    usage: Maneuver
    distance: 15 burst
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: Each target must be dragonsealed. The dragon chooses a direction and
          vertical slides each target 10 squares in that direction, ignoring
          stability. A target who strikes an obstacle takes damage as if they
          had fallen the forced movement distance.
  - type: feature
    feature_type: ability
    name: Field Collapse
    icon: ❗️
    keywords:
      - "-"
    usage: Free triggered action
    distance: Self
    target: Self
    trigger: The dragon takes damage from an ability while the area of their
      Voidshroud Wyrmscale Aura is 2 or more.
    effects:
      - name: Effect
        effect: The dragon halves the damage. Each enemy and object in the area of the
          dragon's Voidshroud Wyrmscale Aura trait takes 5 sonic damage and is
          pulled up to 5 squares toward the dragon. The area of the wyrmscale
          aura then resets to 1.
  - type: feature
    feature_type: ability
    name: A Hero Faces the Void
    icon: ❗️
    cost: 2 Malice
    keywords:
      - Magic
      - Ranged
    usage: Free triggered action
    distance: Ranged 5
    target: The triggering creature
    trigger: A creature within distance spends their Heroic Resource to use an ability.
    effects:
      - roll: Power Roll + 5
        tier1: 10 psychic damage; P < 4 frightened (save ends)
        tier2: 16 psychic damage; P < 5 frightened (save ends)
        tier3: 20 psychic damage; P < 6 frightened (save ends)
      - name: Effect
        effect: While frightened this way, the target can't use the triggering ability.
  - type: feature
    feature_type: ability
    name: Impactful Arrival
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
      - Magic
    usage: "-"
    distance: 1-mile burst
    target: Each creature and object in the area
    effects:
      - name: Effect
        effect: Each target takes 30 fire damage, and if they have M < 5, they are
          knocked prone.
      - name: Special
        effect: The dragon can use this ability before the encounter begins.
  - type: feature
    feature_type: ability
    name: Burning Aurora
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - "-"
    usage: "-"
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: Until the end of the encounter, each enemy who is dragonsealed and
          weakened and who the dragon has line of effect to loses 1 of their
          Heroic Resource at the start of each of their turns (to a minimum of
          0). The dragon then uses their Cosmic Tail Ray ability with a double
          edge, targeting four creatures or objects.
  - type: feature
    feature_type: ability
    name: Voidlight Breath
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Area
      - Magic
    usage: "-"
    distance: ∞ x 3 line within 1
    target: Each enemy and object in the area
    effects:
      - name: Effect
        effect: Each target makes an Agility test.
        tier1: 25 damage; I < 6 the target is annihilated
        tier2: 21 damage; I < 5 the target is annihilated
        tier3: 15 damage; I < 4 the target is annihilated
      - effect: An annihilated target must make the test again, decreasing the potency
          for themself by 2 each time they are annihilated. A creature reduced
          to 0 Stamina by this dies and their soul is destroyed.
  - type: feature
    feature_type: trait
    name: Liftoff
    icon: ⭐️
    cost: 3 Malice
    effects:
      - effect: The next time the dragon uses their Crescent Claws ability, they can
          also slide the target up to 5 squares. If the target is dragonsealed,
          the dragon can vertical slide them instead.
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
    name: Starfall
    icon: 🔳
    cost: 5 Malice
    effects:
      - effect: The dragon drops stars into five 2 cubes anywhere on the encounter map.
          The area is difficult terrain, and each creature and object in the
          area when it appears makes an **Agility test**.
        tier1: 20 holy damage; slowed (save ends), prone
        tier2: 16 holy damage; slowed (save ends)
        tier3: 10 holy damage
  - type: feature
    feature_type: trait
    name: Event Horizon
    icon: ☠️
    cost: 10 Malice
    effects:
      - effect: A black hole manifests as a 1 cube within 20 squares of the dragon in an
          unoccupied space. Each creature who has M < 5 and each object of size
          3 or smaller is vertical pulled 2 squares toward the area at the start
          of each round, ignoring stability. Any creature who starts their turn
          in the area or any object in the area at the end of the round suffers
          the effect of the dragon's Voidlight Breath ability, and the black
          hole disappears.
~~~