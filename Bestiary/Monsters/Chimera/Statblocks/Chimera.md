---
agility: 2
ancestry:
- Beast
- Chimera
ev: '60'
file_basename: Chimera
file_dpath: Monsters/Chimera/Statblocks
free_strike: 6
intuition: 1
item_id: chimera
item_index: '01'
item_name: Chimera
level: 3
might: 3
presence: 0
reason: -2
roles:
- Solo
scc:
- mcdm.monsters.v1:monster:chimera
scdc:
- 1.1.1:2:01
size: '2'
source: mcdm.monsters.v1
speed: 10
stability: 1
stamina: '300'
type: monster
---

```ds-statblock
name: Chimera
level: 3
roles:
  - Solo
ancestry:
  - Beast
  - Chimera
ev: "60"
stamina: "300"
immunities:
  - Fire 6
speed: 10
movement: Fly
size: "2"
stability: 1
free_strike: 6
might: 3
agility: 2
reason: -2
intuition: 1
presence: 0
traits:
  - name: Solo Monster
    effects:
      - effect: At the end of each of their turns, the chimera can take 5 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
        name: End Effect
      - effect: The chimera can take two turns each round. They can't take turns
          consecutively.
        name: Solo Turns
  - name: Volant
    effects:
      - effect: When the chimera makes a creature winded or reduces them to 0 Stamina,
          they can move their speed toward an enemy.
abilities:
  - name: Bite
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
      - roll: Power Roll + 3
        t1: 9 damage
        t2: 13 damage
        t3: 16 damage
      - effect: This strike deals an extra 3 damage if it gains an edge or has a double
          edge.
        name: Effect
  - name: Dragon's Eruption
    icon: 🔳
    cost: 5 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    type: Main action
    distance: 3 cube within 10
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        t1: 3 fire damage; A < 1 3 fire damage
        t2: 5 fire damage; A < 2 5 fire damage
        t3: 7 fire damage; A < 3 7 fire damage
  - name: Roar
    icon: ❇️
    cost: 5 Malice
    keywords:
      - Area
      - Magic
    type: Main action
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        t1: 4 psychic damage
        t2: 8 psychic damage; I < 2 frightened (save ends)
        t3: 10 psychic damage; I < 3 frightened (save ends)
  - name: Lion's Toss
    icon: 🗡
    keywords:
      - Melee
      - Weapon
    type: Maneuver
    distance: Melee 2
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        t1: Vertical push 2
        t2: Vertical push 3
        t3: Vertical push 5
  - name: Ram's Defiance
    icon: ❗️
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Triggered action
    distance: Melee 2
    target: The triggering creature
    trigger: A creature makes a strike against the chimera and obtains a tier 1 outcome.
    effects:
      - name: Effect
        effect: The chimera shifts up to 5 squares. If they end this shift within
          distance of the target, make a power roll.
      - effect: "**Power Roll + 3**"
        t1: 6 damage; M < 1 slowed (save ends)
        t2: 8 damage; prone; M < 2 slowed (save ends)
        t3: 10 damage; prone; M < 3 slowed (save ends)
  - name: Overture of Destruction
    icon: ☠️
    cost: Villain Action 1
    keywords:
      - Area
    type: "-"
    distance: 1 burst
    target: Each enemy in the area
    effects:
      - effect: The chimera can use Bite and Lion's Toss against each target.
        name: Effect
  - name: Fire Solo
    icon: ☠️
    cost: Villain Action 2
    keywords:
      - "-"
    type: "-"
    distance: Self
    target: Self
    effects:
      - effect: The chimera uses Dragon's Eruption and Roar without spending Malice.
        name: Effect
  - name: Chorus of Destruction
    icon: ☠️
    cost: Villain Action 3
    keywords:
      - "-"
    type: "-"
    distance: Self
    target: Self
    effects:
      - effect: The chimera uses Roar, then shifts up to their speed and can make a free
          strike against each enemy who comes adjacent to them during the shift.
          When the chimera ends this shift, they use Dragon's Eruption. The use
          of these abilities as part of this villain action costs no Malice.
        name: Effect
```