---
agility: 1
ancestry:
- Construct
- Multivok
- Soulless
- Valok
ev: '44'
file_basename: Multivok Chief
file_dpath: Monsters/Valok/Statblocks
free_strike: 9
intuition: 1
item_id: multivok-chief
item_index: '332'
item_name: Multivok Chief
level: 9
might: 4
presence: -3
reason: -2
roles:
- Elite Support
scc:
- mcdm.monsters.v1:monster:multivok-chief
scdc:
- 1.1.1:2:332
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 3
stamina: '220'
type: monster
---

```ds-statblock
name: Multivok Chief
level: 9
roles:
  - Elite Support
ancestry:
  - Construct
  - Multivok
  - Soulless
  - Valok
ev: "44"
stamina: "220"
speed: 5
size: 1L
stability: 3
free_strike: 9
might: 4
agility: 1
reason: -2
intuition: 1
presence: -3
traits:
  - name: Multivok Maintenance
    effects:
      - effect: At the start of the chief's turn, each servok within 2 squares of them
          regains 15 Stamina.
  - name: Crafted to Perfection
    effects:
      - effect: The chief's shape can't be changed by any external effect
  - name: Valiar Might
    effects:
      - effect: While the chief isn't bleeding, weakened, or winded, any power roll made
          against them is automatically a tier 1 outcome. A critical hit still
          grants its additional main action.
abilities:
  - name: Pneumatic Punch
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        t1: 13 damage; push 3
        t2: 18 damage; push 5
        t3: 22 damage; push 8
  - name: Targeting Beam
    cost: 3 Malice
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        t1: 15 damage; A < 2 slowed (save ends)
        t2: 21 damage; A < 3 slowed (save ends)
        t3: 26 damage; A < 4 slowed (save ends)
      - effect: This damage can't be reduced in any way. While a target is slowed this
          way, any strike against them has a double edge.
  - name: Chief's Command
    keywords:
      - Ranged
    type: Maneuver
    distance: Ranged 5
    target: One ally
    effects:
      - effect: The target shifts up to their speed and can use a main action
  - name: Quick Shield
    keywords:
      - Ranged
    type: Triggered action
    distance: Ranged 10
    target: The triggering creature
    trigger: The chief or an ally within distance is subject to an effect that can
      be ended by a saving throw or that ends at the end of their turn.
    effects:
      - effect: The target gains 15 temporary Stamina. Each time this triggered action
          is used, the amount of temporary Stamina received decreases by 3 (to a
          minimum of 0).
```