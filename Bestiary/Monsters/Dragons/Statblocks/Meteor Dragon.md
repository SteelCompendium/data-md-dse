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
item_index: '344'
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
- 1.1.1:2:344
size: '3'
source: mcdm.monsters.v1
speed: 15
stability: 6
stamina: '650'
type: monster
---

~~~ds-statblock
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
traits:
  - name: Solo Monster
    effects:
      - effect: At the end of each of their turns, the dragon can take 20 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
        name: End Effect
      - effect: The dragon can take two turns each round. They can't take turns
          consecutively.
        name: Solo Turns
  - name: Voidshroud Wyrmscale Aura
    effects:
      - effect: The dragon's scales create a 1 aura of void space around them. Any enemy
          who starts their turn in the area takes 10 cold damage and is
          suffocating. Each time the dragon takes damage, the area of the aura
          increases by 1 (to a maximum of 5), and they deal an extra 5 damage
          the next time they use an ability that deals rolled damage.
  - name: Crescent Claws
    effects:
      - effect: Once per turn, the dragon chooses a target within 3 squares. The dragon
          can make a free strike against the target, and ignores banes when
          using abilities against the target until the start of their next turn.
  - name: Liftoff
    effects:
      - effect: The next time the dragon uses their Crescent Claws ability, they can
          also slide the target up to 5 squares. If the target is dragonsealed,
          the dragon can vertical slide them instead.
  - name: Solo Action
    effects:
      - effect: The dragon takes an additional main action on their turn. They can use
          this feature even if they are dazed.
  - name: Starfall
    effects:
      - effect: The dragon drops stars into five 2 cubes anywhere on the encounter map.
          The area is difficult terrain, and each creature and object in the
          area when it appears makes an **Agility test**.
        t1: 20 holy damage; slowed (save ends), prone
        t2: 16 holy damage; slowed (save ends)
        t3: 10 holy damage
  - name: Event Horizon
    effects:
      - effect: A black hole manifests as a 1 cube within 20 squares of the dragon in an
          unoccupied space. Each creature who has M < 5 and each object of size
          3 or smaller is vertical pulled 2 squares toward the area at the start
          of each round, ignoring stability. Any creature who starts their turn
          in the area or any object in the area at the end of the round suffers
          the effect of the dragon's Voidlight Breath ability, and the black
          hole disappears.
abilities:
  - name: Gravity Well
    icon: 🔳
    cost: Signature Ability
    keywords:
      - Area
      - Magic
      - Ranged
    type: Main action
    distance: 4 cube within 10
    target: Each creature and object in the area
    effects:
      - name: Effect
        effect: Each target makes a **Might test**.
        t1: 20 sonic damage; the target is dragonsealed (save ends)
        t2: 16 sonic damage; the target is dragonsealed (save ends)
        t3: 10 sonic damage
      - effect: A dragonsealed target emits a golden aura, and takes 2 damage per square
          moved when falling or when force moved into an obstacle.
  - name: Cosmic Tail Ray
    icon: ⚔️
    keywords:
      - Magic
      - Melee
      - Ranged
      - Strike
    type: Main action
    distance: Melee 2 or ranged 15
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 5
        t1: 15 holy damage; A < 4 weakened (save ends)
        t2: 21 holy damage; A < 5 weakened (save ends)
        t3: 25 holy damage; A < 6 weakened (save ends)
      - effect: If a target made weakened this way is already weakened, they are instead
          dazed until the end of their next turn.
        name: Effect
  - name: Investiture of Gravity
    icon: ❇️
    cost: 5 Malice
    keywords:
      - Area
      - Magic
    type: Maneuver
    distance: 15 burst
    target: Each enemy in the area
    effects:
      - effect: Each target must be dragonsealed. The dragon chooses a direction and
          vertical slides each target 10 squares in that direction, ignoring
          stability. A target who strikes an obstacle takes damage as if they
          had fallen the forced movement distance.
        name: Effect
  - name: Field Collapse
    icon: ❗️
    keywords:
      - "-"
    type: Free triggered action
    distance: Self
    target: Self
    trigger: The dragon takes damage from an ability while the area of their
      Voidshroud Wyrmscale Aura is 2 or more.
    effects:
      - effect: The dragon halves the damage. Each enemy and object in the area of the
          dragon's Voidshroud Wyrmscale Aura trait takes 5 sonic damage and is
          pulled up to 5 squares toward the dragon. The area of the wyrmscale
          aura then resets to 1.
        name: Effect
  - name: A Hero Faces the Void
    icon: ❗️
    cost: 2 Malice
    keywords:
      - Magic
      - Ranged
    type: Free triggered action
    distance: Ranged 5
    target: The triggering creature
    trigger: A creature within distance spends their Heroic Resource to use an ability.
    effects:
      - roll: Power Roll + 5
        t1: 10 psychic damage; P < 4 frightened (save ends)
        t2: 16 psychic damage; P < 5 frightened (save ends)
        t3: 20 psychic damage; P < 6 frightened (save ends)
      - effect: While frightened this way, the target can't use the triggering ability.
        name: Effect
  - name: Impactful Arrival
    icon: ☠️
    cost: Villain Action 1
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 1-mile burst
    target: Each creature and object in the area
    effects:
      - effect: Each target takes 30 fire damage, and if they have M < 5, they are
          knocked prone.
        name: Effect
      - effect: The dragon can use this ability before the encounter begins.
        name: Special
  - name: Burning Aurora
    icon: ☠️
    cost: Villain Action 2
    keywords:
      - "-"
    type: "-"
    distance: Self
    target: Self
    effects:
      - effect: Until the end of the encounter, each enemy who is dragonsealed and
          weakened and who the dragon has line of effect to loses 1 of their
          Heroic Resource at the start of each of their turns (to a minimum of
          0). The dragon then uses their Cosmic Tail Ray ability with a double
          edge, targeting four creatures or objects.
        name: Effect
  - name: Voidlight Breath
    icon: ☠️
    cost: Villain Action 3
    keywords:
      - Area
      - Magic
    type: "-"
    distance: ∞ x 3 line within 1
    target: Each enemy and object in the area
    effects:
      - name: Effect
        effect: Each target makes an Agility test.
        t1: 25 damage; I < 6 the target is annihilated
        t2: 21 damage; I < 5 the target is annihilated
        t3: 15 damage; I < 4 the target is annihilated
      - effect: An annihilated target must make the test again, decreasing the potency
          for themself by 2 each time they are annihilated. A creature reduced
          to 0 Stamina by this dies and their soul is destroyed.
~~~