---
agility: 3
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '48'
file_basename: Soulbinder Psyche
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 10
intuition: 4
item_id: soulbinder-psyche
item_index: '389'
item_name: Soulbinder Psyche
level: 10
might: 1
presence: 5
reason: 3
roles:
- Elite Hexer
scc:
- mcdm.monsters.v1:monster:soulbinder-psyche
scdc:
- 1.1.1:2:389
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '220'
type: monster
---

~~~ds-statblock
name: Soulbinder Psyche
level: 10
roles:
  - Elite Hexer
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "48"
stamina: "220"
speed: 5
movement: Fly, hover
size: 1M
stability: 1
free_strike: 10
might: 1
agility: 3
reason: 3
intuition: 4
presence: 5
traits:
  - name: Immortal Soul
    effects:
      - effect: When Psyche is reduced to 0 Stamina, her spirit surrounds the nearest
          war dog, who has damage immunity 2, deals an extra 5 damage on
          strikes, and can use the following Immortal Flare maneuver until the
          end of the encounter. That war dog also gains the Immortal Soul trait,
          and transfers this effect to the nearest war dog when they die.
abilities:
  - name: Soulbind
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 5
        t1: 15 holy damage; R < 3 the target is soulbound (save ends)
        t2: 20 holy damage; R < 4 the target is soulbound (save ends)
        t3: 24 holy damage; R < 5 the target is soulbound (save ends)
      - effect: A soulbound creature can't benefit from edges or double edges, and can't
          gain or use surges.
        name: Effect
  - name: Soulstorm
    icon: 🔳
    cost: 2 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    type: Main action
    distance: 3 cube within 10
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 5
        t1: 8 corruption damage; P < 3 weakened (EoT)
        t2: 12 corruption damage; P < 4 weakened (EoT)
        t3: 15 corruption damage; P < 5 weakened (EoT)
      - effect: The area is difficult terrain until the start of Psyche's next turn At
          the start of each of her turns, Psyche can use a maneuver to main-
          tain this effect, move the area up to 5 squares, and make the power
          roll against each creature in the area's new location.
        name: Effect
      - effect: Until the start of Psyche's next turn, if this ability makes a creature
          weakened, that creature is also soulbound (save ends; see Soulbind
          above).
        cost: 1 Malice
  - name: Command the Awakened
    icon: ❇️
    keywords:
      - Magic
      - Ranged
    type: Maneuver
    distance: 5 burst
    target: Each soulbound enemy in the area
    effects:
      - effect: Each target takes 5 damage from a self-inflicted wound, and if they have
          M < 4 Psyche slides them up to 5 squares.
        name: Effect
  - name: Spirit Form
    icon: ❗️
    keywords:
      - "-"
    type: Triggered action
    distance: Self
    target: Self
    trigger: An enemy moves within 2 squares of Psyche.
    effects:
      - effect: Psyche moves up to 5 squares, and has damage immunity 5 and ignores
          difficult terrain during this movement. The first time she moves
          through any creature during this movement, that creature takes 5
          corruption damage.
        name: Effect
  - name: Vengeance for the Slain
    icon: ❗️
    keywords:
      - Ranged
    type: Free triggered action
    distance: Ranged 10
    target: One enemy
    trigger: A war dog within distance is made winded or reduced to 0 Stamina.
    effects:
      - effect: The target loses all their surges and takes 5 corruption damage.
        name: Effect
      - effect: The target also takes a bane on their next strike.
        cost: 1 Malice
  - name: Immortal Flare
    icon: 🏹
    keywords:
      - Magic
      - Ranged
    type: Maneuver
    distance: Ranged 10
    target: One creature or object
    effects:
      - effect: The target takes 10 psychic damage.
        name: Effect
~~~