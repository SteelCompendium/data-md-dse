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
traits:
  - name: End Effect
    effects:
      - effect: At the end of each of their turns, the maestro can take 5 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
abilities:
  - name: Cacophony
    icon: ❇️
    cost: Signature Ability
    keywords:
      - Area
      - Magic
    type: Main action
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        t1: 3 sonic damage; slide 1, the maestro can shift 1 square
        t2: 6 sonic damage; slide 3, the maestro shifts up to 3 squares
        t3: 8 sonic damage; slide 5, the maestro shifts up to 5 squares
      - effect: Each ally within distance can use Ready Rodent as a free triggered
          action once before the end of the round.
        name: Effect
  - name: Tempo Changer
    icon: 🏹
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Maneuver
    distance: Ranged 10
    target: Two enemies
    effects:
      - roll: Power Roll + 3
        t1: P < 1 slowed (save ends)
        t2: P < 2 slowed (save ends)
        t3: P < 3 slowed (save ends)
      - effect: Each ally within 3 squares of any target has a +2 bonus to speed until
          the end of their next turn.
        cost: 3 Malice
  - name: Ever-Ready Rodent
    icon: ❗️
    cost: 2 Malice
    keywords:
      - Magic
      - Ranged
    type: Free triggered action
    distance: Ranged 5
    target: The triggering creature
    trigger: A creature within distance deals damage to an ally or takes damage from
      an ally.
    effects:
      - effect: The maestro makes a free strike against the target.
        name: Effect
  - name: Overture
    icon: ☠️
    cost: Villain Action 1
    keywords:
      - Area
    type: "-"
    distance: 10 burst
    target: Each ally in the area
    effects:
      - effect: Each target can shift up to their speed or take the Defend action.
        name: Effect
  - name: Solo Act
    icon: ☠️
    cost: Villain Action 2
    keywords:
      - Ranged
    type: "-"
    distance: Ranged 15
    target: One creature
    effects:
      - effect: Until the end of their next turn, the target halves any damage they
          take, gains a +4 damage bonus to strikes, and has their speed doubled.
        name: Effect
  - name: Rondo of Rat
    icon: ☠️
    cost: Villain Action 3
    keywords:
      - Area
    type: "-"
    distance: 10 burst
    target: Each dead ally in the area
    effects:
      - effect: Each target stands, makes a free strike, then falls dead again. Any ally
          of the targets can use Ready Rodent as a free triggered action once in
          conjunction with these free strikes.
        name: Effect
~~~