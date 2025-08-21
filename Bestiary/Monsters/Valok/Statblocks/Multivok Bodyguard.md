---
agility: 0
ancestry:
- Construct
- Multivok
- Soulless
- Valok
ev: '44'
file_basename: Multivok Bodyguard
file_dpath: Monsters/Valok/Statblocks
free_strike: 9
intuition: 1
item_id: multivok-bodyguard
item_index: '328'
item_name: Multivok Bodyguard
level: 9
might: 4
presence: -4
reason: -2
roles:
- Elite Defender
scc:
- mcdm.monsters.v1:monster:multivok-bodyguard
scdc:
- 1.1.1:2:328
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 5
stamina: '240'
type: monster
---

```ds-statblock
name: Multivok Bodyguard
level: 9
roles:
  - Elite Defender
ancestry:
  - Construct
  - Multivok
  - Soulless
  - Valok
ev: "44"
stamina: "240"
speed: 5
size: "2"
stability: 5
free_strike: 9
might: 4
agility: 0
reason: -2
intuition: 1
presence: -4
traits:
  - name: Multivok Maintenance
    effects:
      - effect: At the start of the bodyguard's turn, each servok within 2 squares of
          them regains 15 Stamina.
  - name: Crafted to Perfection
    effects:
      - effect: The bodyguard's shape can't be changed by any external effect
  - name: Valiar Might
    effects:
      - effect: While the bodyguard isn't bleeding, weakened, or winded, any power roll
          made against them is automatically a tier 1 outcome. A critical hit
          still grants its additional main action.
abilities:
  - name: Gatling Bolt Gun
    cost: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        t1: 13 damage
        t2: 18 damage
        t3: 22 damage; A < 4 bleeding (save ends)
  - name: Valiar Axe
    cost: 3 Malice
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        t1: 15 damage; M < 2 weakened (save ends)
        t2: 21 damage; M < 3 weakened (save ends)
        t3: 26 damage; prone; M < 4 weakened (save ends)
      - effect: The bodyguard has a double edge on this ability if it was previously
          used against the same target in this encounter.
        name: Effect
  - name: Magnetic Pull
    keywords:
      - Area
    type: Maneuver
    distance: 10 burst
    target: Each enemy and object in the area
    effects:
      - effect: This ability targets only metal-clad enemies and metal objects of size 3
          or smaller.
        name: Special
      - effect: Each target is pulled up to 8 squares, or if they have M < 3, they are
          pulled up to 15 squares. The bodyguard can make a free strike against
          each target who ends this forced movement adjacent to them.
        name: Effect
  - name: Valiar Cloak
    keywords:
      - Melee
    type: Triggered action
    distance: Melee 2
    target: Self
    trigger: One ally within distance is targeted by an enemy's ability. The
      bodyguard can use this ability after seeing the outcome of the power roll.
    effects:
      - effect: The bodyguard becomes the triggering ability's target instead.
        name: Effect
```