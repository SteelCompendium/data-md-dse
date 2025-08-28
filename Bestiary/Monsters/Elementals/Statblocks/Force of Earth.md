---
agility: -1
ancestry:
- Elemental
ev: '20'
file_basename: Force of Earth
file_dpath: Monsters/Elementals/Statblocks
free_strike: 6
intuition: 1
item_id: force-of-earth
item_index: '326'
item_name: Force of Earth
level: 3
might: 2
presence: 2
reason: 0
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:force-of-earth
scdc:
- 1.1.1:2:326
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '132'
type: monster
---

~~~ds-statblock
name: Force of Earth
level: 3
roles:
  - Elite Brute
ancestry:
  - Elemental
ev: "20"
stamina: "132"
speed: 5
movement: Burrow
size: "2"
stability: 2
free_strike: 6
might: 2
agility: -1
reason: 0
intuition: 1
presence: 2
traits:
  - name: Fickle and Free
    effects:
      - effect: The force can't be restrained, slowed, or knocked prone, and they ignore
          difficult terrain.
  - name: Primordial Strength
    effects:
      - effect: The force's strikes gain a +6 damage bonus against objects.
  - name: Stone Swim
    effects:
      - effect: The force can burrow through stone, but can't drag other creatures
          underground when they do so.
abilities:
  - name: Slam Into Dirt
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        t1: 8 damage
        t2: 12 damage; M < 1 restrained (save ends)
        t3: 15 damage; M < 2 restrained (save ends)
      - effect: The target's space is difficult terrain.
        name: Effect
  - name: Convocation of Quartz
    icon: 🏹
    keywords:
      - Magic
      - Ranged
    type: Maneuver
    distance: Ranged 5
    target: Self or one elemental
    effects:
      - effect: Until the start of the force's next turn, any melee strike made against
          the target takes a bane if it doesn't already have a bane or double
          bane.
        name: Effect
      - effect: Until the end of the encounter, the target grows a carapace of stone.
          They have a +3 bonus to stability and gain 15 temporary Stamina.
        cost: 3 Malice
  - name: Break Armor
    icon: ❗️
    cost: 1 Malice
    keywords:
      - "-"
    type: Triggered action
    distance: Self
    target: Self
    trigger: The force takes damage.
    effects:
      - effect: The force halves the damage, and has damage weakness 3 and a +3 bonus to
          speed until the end of the encounter. This damage weakness increases
          by 3 each time the force uses this ability in the same encounter.
        name: Effect
~~~