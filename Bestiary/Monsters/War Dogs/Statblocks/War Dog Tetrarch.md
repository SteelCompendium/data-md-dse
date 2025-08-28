---
agility: 3
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '32'
file_basename: War Dog Tetrarch
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 7
intuition: 3
item_id: war-dog-tetrarch
item_index: '361'
item_name: War Dog Tetrarch
level: 6
might: 4
presence: 4
reason: 2
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:war-dog-tetrarch
scdc:
- 1.1.1:2:361
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 2
stamina: '180'
type: monster
---

```ds-statblock
name: War Dog Tetrarch
level: 6
roles:
  - Leader
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "32"
stamina: "180"
speed: 7
size: 1M
stability: 2
free_strike: 7
might: 4
agility: 3
reason: 2
intuition: 3
presence: 4
traits:
  - name: End Effect
    effects:
      - effect: At the end of each of their turns, the tetrarch can take 10 damage to
          end one effect on them that can be ended by a saving throw. This
          damage can't be reduced in any way.
abilities:
  - name: Houndblade
    icon: ⚔️
    cost: Signature Ability
    keywords:
      - Charge
      - Melee
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1 or ranged 3
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        t1: 11 damage
        t2: 16 damage; taunted (EoT)
        t3: 19 damage; taunted (EoT)
      - effect: A creature taunted this way takes a bane on strikes.
        name: Effect
      - effect: Each target loses 1d3 Recoveries.
        cost: 3 Malice
  - name: Get Them, You Dolts! 1 Malice per target
    icon: 🏹
    keywords:
      - Ranged
    type: Maneuver
    distance: Ranged 10
    target: Three creatures
    effects:
      - effect: Each target shifts up to their speed and can make a free strike. If the
          free strike targets an enemy taunted by the tetrarch, it deals an
          extra 4 damage.
        name: Effect
  - name: Sneering Disregard
    icon: ❗️
    keywords:
      - Ranged
    type: Triggered action
    distance: Ranged 10
    target: The triggering creature
    trigger: A creature within distance who is not taunted by the tetrarch targets
      the tetrarch with a power roll.
    effects:
      - effect: The power roll has a double bane. If the target obtains a tier 1
          outcome, the tetrarch ignores any of the power roll's effects other
          than damage and the target is frightened of the tetrarch (save ends).
        name: Effect
  - name: Enter the Fray
    icon: ☠️
    cost: Villain Action 1
    keywords:
      - Area
    type: "-"
    distance: 2 burst
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: The tetrarch can jump up to 7 squares before using this ability.
      - roll: Power Roll + 4
        t1: Push 2; I < 2 frightened (save ends)
        t2: Push 4; I < 3 frightened (save ends)
        t3: Push 5; I < 4 frightened (save ends)
  - name: Lay Waste
    icon: ☠️
    cost: Villain Action 2
    keywords:
      - Area
      - Ranged
      - Weapon
    type: "-"
    distance: Five 2 cubes within 20
    target: Each creature and object in the area
    effects:
      - roll: Power Roll + 4
        t1: 7 fire damage; A < 2 slowed (EoT)
        t2: 13 fire damage; A < 3 slowed (save ends)
        t3: 16 fire damage; A < 4 slowed (save ends)
      - effect: The area is set ablaze until the end of the encounter. While ablaze, the
          area is difficult terrain, and any creature takes 2 fire damage for
          each square in the area they enter for the first time in a round
        name: Effect
  - name: You Would Dare?!
    icon: ☠️
    cost: Villain Action 3
    keywords:
      - "-"
    type: "-"
    distance: Self
    target: Self
    effects:
      - effect: Until the end of the encounter, the tetrarch has damage immunity 2, and
          their Houndblade ability targets three creatures or objects.
        name: Effect
```