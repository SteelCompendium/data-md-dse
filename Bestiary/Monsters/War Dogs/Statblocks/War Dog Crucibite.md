---
agility: 2
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '3'
file_basename: War Dog Crucibite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 2
intuition: 0
item_id: war-dog-crucibite
item_index: '355'
item_name: War Dog Crucibite
level: 1
might: 0
presence: 0
reason: 0
roles:
- Horde Artillery
scc:
- mcdm.monsters.v1:monster:war-dog-crucibite
scdc:
- 1.1.1:2:355
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '10'
type: monster
---

~~~ds-statblock
name: War Dog Crucibite
level: 1
roles:
  - Horde Artillery
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "3"
stamina: "10"
immunities:
  - Fire 2
speed: 5
size: 1M
stability: 0
free_strike: 2
might: 0
agility: 2
reason: 0
intuition: 0
presence: 0
traits:
  - name: Loyalty Collar
    effects:
      - effect: When the crucibite is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 1d6 damage to each adjacent enemy and object.
abilities:
  - name: Flamebelcher
    icon: 🔳
    cost: Signature Ability
    keywords:
      - Area
      - Weapon
    type: Main action
    distance: 5 x 1 line within 1
    target: Each creature and object in the area
    effects:
      - roll: Power Roll + 2
        t1: 2 fire damage
        t2: 4 fire damage
        t3: 5 fire damage
      - effect: The area is covered in sticky fire until the start of the crucibite's
          next turn. Any creature who enters the area for the first time in a
          round or starts their turn there takes 2 fire damage
        name: Effect
      - effect: The area becomes a 10 x 1 line, and if any ally of the crucibite is in
          the area when it is created, the ability deals an extra 2 damage to
          each target.
        cost: 3 Malice
  - name: Posthumous Promotion
    icon: 🏹
    keywords:
      - Magic
      - Ranged
    type: Maneuver
    distance: Ranged 10
    target: One war dog
    effects:
      - effect: If the target has a loyalty collar, they are reduced to 0 Stamina.
        name: Effect
~~~