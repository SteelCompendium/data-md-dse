---
agility: 3
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '8'
file_basename: War Dog Arachnite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 4
intuition: 2
item_id: war-dog-arachnite
item_index: '380'
item_name: War Dog Arachnite
level: 6
might: 0
presence: 1
reason: 2
roles:
- Horde Artillery
scc:
- mcdm.monsters.v1:monster:war-dog-arachnite
scdc:
- 1.1.1:2:380
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '35'
type: monster
---

~~~ds-statblock
name: War Dog Arachnite
level: 6
roles:
  - Horde Artillery
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "8"
stamina: "35"
immunities:
  - Psychic 6
speed: 5
movement: Climb
size: 1L
stability: 0
free_strike: 4
might: 0
agility: 3
reason: 2
intuition: 2
presence: 1
traits:
  - name: Eight-Eyed Sight
    effects:
      - effect: At the start of each of their turns, the arachnite automatically knows
          the location of each hidden creature within 10 squares of them.
  - name: Loyalty Collar
    effects:
      - effect: When the arachnite is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 2d6 damage to each adjacent enemy and object.
abilities:
  - name: Longarm Shrikegun
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 15
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        t1: 7 damage
        t2: 9 damage
        t3: 11 damage; A < 3 bleeding (save ends)
      - effect: "This ability ignores cover and concealment. The arachnite chooses one
          of the following damage types when making the strike: acid, cold,
          fire, lightning, poison, psychic, or sonic"
        name: Effect
      - effect: The arachnite can use this ability as if they were in the space of any
          ally within distance.
        cost: 2 Malice
  - name: Web Vial
    icon: 🔳
    keywords:
      - Area
      - Ranged
    type: Maneuver
    distance: 2 cube within 10
    target: Special
    effects:
      - effect: The area is difficult terrain until the end of the encounter
        name: Effect
~~~