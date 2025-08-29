---
agility: 2
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '48'
file_basename: Castellan Hoplon
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 0
intuition: 3
item_id: castellan-hoplon
item_index: '387'
item_name: Castellan Hoplon
level: 10
might: 5
presence: 4
reason: 4
roles:
- Elite Defender
scc:
- mcdm.monsters.v1:monster:castellan-hoplon
scdc:
- 1.1.1:2:387
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '2603'
type: monster
---

~~~ds-statblock
name: Castellan Hoplon
level: 10
roles:
  - Elite Defender
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "48"
stamina: "2603"
immunities:
  - Damage 3
speed: 5
size: 1M
stability: 1
free_strike: 0
might: 5
agility: 2
reason: 4
intuition: 3
presence: 4
traits:
  - name: Hold the Line
    effects:
      - effect: Each ally within 3 squares of Hoplon has cover and damage immunity 2.
  - name: Last Stand
    effects:
      - effect: The first time in an encounter that Hoplon is reduced to 0 Stam- na, he
          instead has 1 Stamina and gains damage immunity 10 until the end of
          his next turn. When Hoplon is reduced to 0 Stamina again, each ally
          within 5 squares of him gains damage immunity 3 and deals an extra 5
          damage on strikes, all until the end of the encounter.
abilities:
  - name: Inspiring Strike
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 5
        t1: 15 damage
        t2: 20 damage; push 3
        t3: 24 damage; push 5
      - effect: Two allies within 10 squares of Hoplon each shift up to their speed,
          then can take the Defend main action or make a free strike.
        name: Effect
  - name: Summon the Onyx Tower
    icon: 🏹
    cost: 5 Malice
    keywords:
      - Ranged
    type: Maneuver
    distance: Ranged 15
    target: Special
    effects:
      - effect: A 10-square-tall tower made of black stone shimmers into being in an
          unoccupied space that is 5 squares on a side. The tower has three
          floors, an entrance in the middle of each side on the ground floor,
          and a crenelated rooftop. Any war dog inside or adjacent to the tower
          has damage immunity 2 and regains 5 Stamina at the start of each of
          their turns, and war dogs inside the tower can observe through and
          have line of effect through its walls. This ability can be used only
          once per encounter.
        name: Effect
  - name: Shield Warden
    icon: ❇️
    cost: 2 Malice
    keywords:
      - Area
    type: Maneuver
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - cost: ≤11
        effect: R < 3 taunted (EoT)
        t2: R < 4 taunted (EoT)
        t3: R < 5 taunted (EoT)
      - effect: Until the start of Hoplon's next turn, any enemy ability that includes
          him as a target takes a bane.
        name: Effect
  - name: Timely Intervention
    icon: ❗️
    keywords:
      - Magic
    type: Triggered action
    distance: Self
    target: Self
    trigger: An enemy within 10 squares targets an ally with an ability.
    effects:
      - effect: Hoplon teleports to an unoccupied space adjacent to the enemy and
          becomes the new target of the ability. He can then make a free strike
          against the enemy, and if that enemy has R < 4 they are taunted until
          the end of their next turn.
        name: Effect
~~~