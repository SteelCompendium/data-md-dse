---
agility: -2
ancestry:
- Construct
- Servok
- Soulless
- Valok
ev: '44'
file_basename: Servok Builder
file_dpath: Monsters/Valok/Statblocks
free_strike: 10
intuition: -1
item_id: servok-builder
item_index: '330'
item_name: Servok Builder
level: 9
might: 4
presence: -5
reason: -4
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:servok-builder
scdc:
- 1.1.1:2:330
size: '3'
source: mcdm.monsters.v1
speed: 5
stability: 8
stamina: '240'
type: monster
---

~~~ds-statblock
name: Servok Builder
level: 9
roles:
  - Elite Brute
ancestry:
  - Construct
  - Servok
  - Soulless
  - Valok
ev: "44"
stamina: "240"
speed: 5
size: "3"
stability: 8
free_strike: 10
might: 4
agility: -2
reason: -4
intuition: -1
presence: -5
traits:
  - name: Servok Siege Machine
    effects:
      - effect: The builder ignores difficult terrain, and their abilities deal an extra
          15 damage to objects.
  - name: Crafted to Perfection
    effects:
      - effect: The builder's shape can't be changed by any external effect
  - name: Valiar Might
    effects:
      - effect: While the builder isn't bleeding, weakened, or winded, any power roll
          made against them is automatically a tier 1 outcome. A critical hit
          still grants its additional main action.
abilities:
  - name: Wrecking Ball
    icon: 🔳
    cost: Signature Ability
    keywords:
      - Area
      - Ranged
      - Weapon
    type: Main action
    distance: 3 cube within 5
    target: Each enemy and object in the area
    effects:
      - name: Effect
        effect: Each target must make either an Agility test or an **Intuition test**.
        t1: 15 damage; push 5, prone
        t2: 12 damage; push 3
        t3: 8 damage
  - name: Construction Arm
    icon: 🗡
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 3
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        t1: 16 damage
        t2: 23 damage; grabbed
        t3: 28 damage; grabbed; M < 4 vertical push 5
  - name: Lay the Foundation
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
    type: Main action
    distance: 6 x 3 line within 1
    target: Special
    effects:
      - name: Effect
        effect: The area is covered in wet concrete and is difficult terrain. An enemy
          who starts their turn in the concrete makes a **Might test**.
        t1: Restrained (EoT)
        t2: Slowed (EoT)
        t3: No effect
  - name: Build Wall
    icon: 🔳
    keywords:
      - Area
      - Ranged
    type: Maneuver
    distance: 6 wall within 3
    target: Special
    effects:
      - effect: The builder creates a concrete wall. They can also remove any unoccupied
          squares of wet concrete within 3 squares of them, creating two
          additional squares of wall for each square of concrete removed.
        name: Effect
  - name: Sputter
    icon: ❗️
    cost: 1 Malice
    keywords:
      - Melee
    type: Free triggered action
    distance: Melee 3
    target: The triggering creature or object
    trigger: A creature or object within distance deals damage to the builder.
    effects:
      - roll: Power Roll + 4
        t1: A < 2 restrained (save ends)
        t2: A < 3 restrained (save ends)
        t3: A < 4 restrained (save ends)
      - effect: While a creature is restrained this way, or if the target is an object,
          the target and their space are encased in wet concrete. A creature no
          longer restrained leaves squares of wet concrete behind.
        name: Effect
~~~