---
agility: 0
ancestry:
- Humanoid
- Soulless
- War Dog
ev: 3 for four minions
file_basename: War Dog Tetherite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 2
intuition: 0
item_id: war-dog-tetherite
item_index: '384'
item_name: War Dog Tetherite
level: 1
might: 2
presence: 0
reason: 0
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster:war-dog-tetherite
scdc:
- 1.1.1:2:384
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '5'
type: monster
---

```ds-statblock
name: War Dog Tetherite
level: 1
roles:
  - Minion Brute
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: 3 for four minions
stamina: "5"
speed: 5
size: 1M
stability: 1
free_strike: 2
with_captain: Gain an edge on strikes
might: 2
agility: 0
reason: 0
intuition: 0
presence: 0
traits:
  - name: Tethered
    effects:
      - effect: A captain attached to a tetherite squad has their stability increased by
          the number of tetherites within 2 squares of them.
  - name: Loyalty Collar
    effects:
      - effect: When the tetherite is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 1d3 damage to each adjacent enemy and object.War Dog
          Malice Level 1+ Malice Features At the start of any war dog's turn,
          you can spend Malice to activate one of the following features.
  - name: Reconstitute
    effects:
      - effect: One war dog acting this turn tears apart a nearby corpse of a humanoid
          and incorporates its body parts into their own. The war dog regains
          Stamina equal to 5 times their level.
  - name: Fodder Run
    effects:
      - effect: Each war dog minion in the encounter shifts up to their speed and can
          make a free strike. A minion who does so is then reduced to 0
abilities:
  - name: Banded Dagger
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        t1: 2 damage
        t2: 4 damage
        t3: 5 damage
  - name: Fire for Effect
    icon: 🔳
    cost: 5 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    type: Maneuver
    distance: 4 cube within 10
    target: Each creature in the area
    effects:
      - name: Effect
        effect: Each target makes an Agility test. The same condition is imposed on each
          affected target.
      - roll: Power Roll + 3
        t1: 5 fire damage; slowed or weakened (save ends
        t2: 5 fire damage; slowed or weakened (EoT
        t3: 5 fire damage
```