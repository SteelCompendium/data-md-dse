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

```ds-statblock
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
traits:
  - name: Solo Monster
    effects:
      - effect: At the end of each of their turns, the bredbeddle can take 5 damage to
          end one effect on them that can be ended by a saving throw. This
          damage can't be reduced in any way.
        name: End Effect
      - effect: The bredbeddle can take two turns each round. They can't take turns
          consecutively.
        name: Solo Turns
  - name: Heady or Not
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
  - name: Resilient Form
    effects:
      - effect: The bredbeddle can't be physically transformed in any way except by
          their Heady or Not trait.
abilities:
  - name: Executioner's Swing
    cost: Signature Ability
    keywords:
      - Area
      - Weapon
    type: Main action
    distance: 2 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        t1: 2 damage; A < 1 bleeding (save ends)
        t2: 4 damage; A < 2 bleeding (save ends)
        t3: 5 damage; A < 3 bleeding (save ends); M < 2 dazed (save ends)
      - effect: The bredbeddle shifts up to 2 squares, and can target additional enemies
          who come within distance of this ability during the shift.
        name: Malice
  - name: Lop
    cost: 3 Malice
    keywords:
      - Magic
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: One creature
    effects:
      - roll: Power Roll + 3
        t1: 9 damage; bleeding (save ends); or if the target has M < 1 they are beheaded
        t2: 13 damage; bleeding (save ends); or if the target has M < 2 they are
          beheaded
        t3: 16 damage; bleeding (save ends); or if the target has M < 3 they are
          beheaded
      - effect: A beheaded target has their head fall into an unoccupied square adjacent
          to the bredbeddle, but they remain alive. While beheaded this way, the
          target is bleeding and has line of effect only to adjacent squares.
          The beheaded target can survive without their head for 24 hours, and
          can reattach their head as a maneuver by entering its square. A target
          who remains beheaded for 24 hours dies.
        name: Effect
  - name: Scramble
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: While the bredbeddle is headless, they shift up to their speed. Each
          time a creature comes adjacent to the bredbeddle during the shift, the
          bredbeddle can push that creature 1 square. Each square the bredbeddle
          exits during the shift is difficult terrain.
        name: Effect
  - name: Headway
    cost: 5 Malice
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Maneuver
    distance: Ranged 20
    target: One creature or object
    effects:
      - name: Effect
        effect: The bredbeddle must have a head in their possession (attached to them or
          not), which they throw at the target. If the head was attached, the
          bredbeddle is left headless.
      - roll: Power Roll + 3
        t1: 9 damage; M < 1 dazed (save ends)
        t2: 13 damage; prone; M < 2 dazed (save ends)
        t3: 16 damage; prone; M < 3 dazed (save ends)
  - name: Envious Imitation
    cost: 2 Malice
    keywords:
      - Magic
    type: Triggered action
    distance: Self
    target: Self
    trigger: A creature targets the bredbeddle with a ranged strike.
    effects:
      - effect: The bredbeddle uses the same ability against the triggering creature
          after the triggering strike is resolved, using that creature's bonus
          to any power rolls they make.
        name: Effect
  - name: Turn Green
    cost: Villain Action 1
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        t1: P < 1 the target turns green (save ends)
        t2: P < 2 the target turns green (save ends)
        t3: P < 3 the target turns green until the end of the encounter
      - effect: Green shadows crawl out from under the bredbeddle's feet and turn each
          target green. The bredbeddle has a double edge on power rolls against
          any target turned green this way.
        name: Effect
  - name: Challenge
    cost: Villain Action 2
    keywords:
      - Ranged
    type: "-"
    distance: Ranged 5
    target: One enemy
    effects:
      - name: Effect
        effect: The bredbeddle points at the target and issues them a challenge. If the
          target refuses, they turn green until the end of the encounter (see
          Turn Green). If the target accepts the challenge, the bredbeddle
          shifts adjacent to the target, who makes a **Might test** with no
          additional modifiers.
        t1: The target is beheaded (see Lop).
        t2: The target makes the test again.
        t3: The target can choose to deal 40 damage to the bredbeddle or remove the
          bredbeddle's head.
  - name: Headlam Rampage
    cost: Villain Action 3
    keywords:
      - Melee
      - Strike
      - Weapon
    type: "-"
    distance: Melee 2
    target: Four creatures
    effects:
      - cost: ≤11
        effect: 6 damage; bleeding (save ends); or if the target has A < 1 they are
          beheaded (see Lop).
        t2: 7 damage; bleeding (save ends); or if the target has A < 2 they are beheaded
        t3: 8 damage; bleeding (save ends); or if the target has A < 3 they are beheaded
```