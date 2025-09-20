---
agility: 0
ancestry:
- Bredbeddle
- Giant
ev: '60'
file_basename: Bredbeddle
file_dpath: Monsters/Bredbeddle/Statblocks
free_strike: 6
intuition: 2
item_id: bredbeddle
item_index: '205'
item_name: Bredbeddle
level: 3
might: 3
presence: 2
reason: -3
roles:
- Solo
scc:
- mcdm.monsters.v1:monster:bredbeddle
scdc:
- 1.1.1:2:205
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 4
stamina: '300'
type: monster
---

~~~ds-statblock
type: statblock
name: Bredbeddle
level: 3
roles:
  - Solo
ancestry:
  - Bredbeddle
  - Giant
ev: "60"
stamina: "300"
speed: 5
size: "2"
stability: 4
free_strike: 6
might: 3
agility: 0
reason: -3
intuition: 2
presence: 2
features:
  - type: feature
    feature_type: trait
    name: Solo Monster
    icon: ☠️
    effects:
      - name: End Effect
        effect: At the end of each of their turns, the bredbeddle can take 5 damage to
          end one effect on them that can be ended by a saving throw. This
          damage can't be reduced in any way.
      - name: Solo Turns
        effect: The bredbeddle can take two turns each round. They can't take turns
          consecutively.
  - type: feature
    feature_type: trait
    name: Heady or Not
    icon: ⭐️
    effects:
      - effect: >-
          While headless, the bredbeddle can move into a space containing a
          severed head and attach it to their neck as a main action. Doing so
          physically transforms the bredbeddle, who takes on the appearance,
          size, weight, and stability of the head's original owner. If the
          bredbeddle takes the form of a creature of size 1L or smaller, the
          distance of their melee and burst area abilities decreases by 1. These
          effects last until the bredbeddle is killed or beheaded, or until the
          head falls off after 24 hours. A head that falls off this way can no
          longer be attached to this bredbeddle.


          A creature must succeed on a **hard Might test** made as a maneuver to
          rip a head off the bredbeddle. If they fail, the bredbeddle can make a
          free strike against them.
  - type: feature
    feature_type: trait
    name: Resilient Form
    icon: ⭐️
    effects:
      - effect: The bredbeddle can't be physically transformed in any way except by
          their Heady or Not trait.
  - type: feature
    feature_type: ability
    name: Executioner's Swing
    icon: ❇️
    ability_type: Signature Ability
    keywords:
      - Area
      - Weapon
    usage: Main action
    distance: 2 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        tier1: 2 damage; A < 1 bleeding (save ends)
        tier2: 4 damage; A < 2 bleeding (save ends)
        tier3: 5 damage; A < 3 bleeding (save ends); M < 2 dazed (save ends)
      - cost: 3 Malice
        effect: The bredbeddle shifts up to 2 squares, and can target additional enemies
          who come within distance of this ability during the shift.
  - type: feature
    feature_type: ability
    name: Lop
    icon: 🗡
    cost: 3 Malice
    keywords:
      - Magic
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 2
    target: One creature
    effects:
      - roll: Power Roll + 3
        tier1: 9 damage; bleeding (save ends); or if the target has M < 1 they are
          beheaded
        tier2: 13 damage; bleeding (save ends); or if the target has M < 2 they are
          beheaded
        tier3: 16 damage; bleeding (save ends); or if the target has M < 3 they are
          beheaded
      - name: Effect
        effect: A beheaded target has their head fall into an unoccupied square adjacent
          to the bredbeddle, but they remain alive. While beheaded this way, the
          target is bleeding and has line of effect only to adjacent squares.
          The beheaded target can survive without their head for 24 hours, and
          can reattach their head as a maneuver by entering its square. A target
          who remains beheaded for 24 hours dies.
  - type: feature
    feature_type: ability
    name: Scramble
    icon: 👤
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: While the bredbeddle is headless, they shift up to their speed. Each
          time a creature comes adjacent to the bredbeddle during the shift, the
          bredbeddle can push that creature 1 square. Each square the bredbeddle
          exits during the shift is difficult terrain.
  - type: feature
    feature_type: ability
    name: Headway
    icon: 🏹
    cost: 5 Malice
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Maneuver
    distance: Ranged 20
    target: One creature or object
    effects:
      - name: Effect
        effect: The bredbeddle must have a head in their possession (attached to them or
          not), which they throw at the target. If the head was attached, the
          bredbeddle is left headless.
      - roll: Power Roll + 3
        tier1: 9 damage; M < 1 dazed (save ends)
        tier2: 13 damage; prone; M < 2 dazed (save ends)
        tier3: 16 damage; prone; M < 3 dazed (save ends)
  - type: feature
    feature_type: ability
    name: Envious Imitation
    icon: ❗️
    cost: 2 Malice
    keywords:
      - Magic
    usage: Triggered action
    distance: Self
    target: Self
    trigger: A creature targets the bredbeddle with a ranged strike.
    effects:
      - name: Effect
        effect: The bredbeddle uses the same ability against the triggering creature
          after the triggering strike is resolved, using that creature's bonus
          to any power rolls they make.
  - type: feature
    feature_type: ability
    name: Turn Green
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
      - Magic
    usage: "-"
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        tier1: P < 1 the target turns green (save ends)
        tier2: P < 2 the target turns green (save ends)
        tier3: P < 3 the target turns green until the end of the encounter
      - name: Effect
        effect: Green shadows crawl out from under the bredbeddle's feet and turn each
          target green. The bredbeddle has a double edge on power rolls against
          any target turned green this way.
  - type: feature
    feature_type: ability
    name: Challenge
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - Ranged
    usage: "-"
    distance: Ranged 5
    target: One enemy
    effects:
      - name: Effect
        effect: The bredbeddle points at the target and issues them a challenge. If the
          target refuses, they turn green until the end of the encounter (see
          Turn Green). If the target accepts the challenge, the bredbeddle
          shifts adjacent to the target, who makes a **Might test** with no
          additional modifiers.
        tier1: The target is beheaded (see Lop).
        tier2: The target makes the test again.
        tier3: The target can choose to deal 40 damage to the bredbeddle or remove the
          bredbeddle's head.
  - type: feature
    feature_type: ability
    name: Headlam Rampage
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Melee
      - Strike
      - Weapon
    usage: "-"
    distance: Melee 2
    target: Four creatures
    effects:
      - roll: Power Roll + 3
        tier1: 6 damage; bleeding (save ends); or if the target has A < 1 they are
          beheaded (see Lop).
        tier2: 7 damage; bleeding (save ends); or if the target has A < 2 they are
          beheaded
        tier3: 8 damage; bleeding (save ends); or if the target has A < 3 they are
          beheaded
~~~