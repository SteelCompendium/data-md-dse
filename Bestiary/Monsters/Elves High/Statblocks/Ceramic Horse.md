---
agility: 2
ancestry:
- Elemental
- High Elf
ev: '6'
file_basename: Ceramic Horse
file_dpath: Monsters/Elves High/Statblocks
free_strike: 3
intuition: 0
item_id: ceramic-horse
item_index: '118'
item_name: Ceramic Horse
level: 1
might: 2
presence: 1
reason: 0
roles:
- Platoon Mount
scc:
- mcdm.monsters.v1:monster:ceramic-horse
scdc:
- 1.1.1:2:118
size: '2'
source: mcdm.monsters.v1
speed: 10
stability: 2
stamina: '30'
type: monster
---

~~~ds-statblock
name: Ceramic Horse
level: 1
roles:
  - Platoon Mount
ancestry:
  - Elemental
  - High Elf
ev: "6"
stamina: "30"
speed: 10
size: "2"
stability: 2
free_strike: 3
might: 2
agility: 2
reason: 0
intuition: 0
presence: 1
traits:
  - name: Shared Otherworldly Grace
    effects:
      - effect: If the ceramic horse's rider has the Otherworldly Grace trait, the
          ceramic horse also has that trait.
abilities:
  - name: Elemental Charge
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 5 damage
        t2: 7 fire damage
        t3: 9 lightning damage; M < 2 prone
  - name: Stomp
    icon: ❇️
    keywords:
      - Area
      - Weapon
    type: Main action
    distance: 1 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        t1: 3 damage
        t2: 5 damage
        t3: 7 damage
      - effect: Any target who is prone takes an extra 2 damage.
        name: Effect
  - name: Buck
    icon: 👤
    cost: 2 Malice
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: The horse's rider
    effects:
      - effect: The horse vertical slides the target up to 3 squares, ignoring
          stability. The target can use a ranged ability at any point during
          this forced movement, and takes no damage if they then fall.
        name: Effect
~~~