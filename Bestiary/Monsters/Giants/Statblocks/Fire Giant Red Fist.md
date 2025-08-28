---
agility: 2
ancestry:
- Fire Giant
- Giant
ev: '44'
file_basename: Fire Giant Red Fist
file_dpath: Monsters/Giants/Statblocks
free_strike: 10
intuition: 2
item_id: fire-giant-red-fist
item_index: '198'
item_name: Fire Giant Red Fist
level: 9
might: 4
presence: 1
reason: 0
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:fire-giant-red-fist
scdc:
- 1.1.1:2:198
size: '4'
source: mcdm.monsters.v1
speed: 8
stability: 5
stamina: '240'
type: monster
---

```ds-statblock
name: Fire Giant Red Fist
level: 9
roles:
  - Elite Brute
ancestry:
  - Fire Giant
  - Giant
ev: "44"
stamina: "240"
immunities:
  - Fire 9
speed: 8
size: "4"
stability: 5
free_strike: 10
might: 4
agility: 2
reason: 0
intuition: 2
presence: 1
traits:
  - name: Searing Skin
    effects:
      - effect: Whenever an adjacent enemy grabs the red fist or uses a melee ability
          against them, that enemy takes 5 fire damage.
abilities:
  - name: Flaming Punch
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 3
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        t1: 14 fire damage; push
        t2: 19 fire damage; push 4; A < 3 burning (save ends)
        t3: 23 fire damage; push 6; A < 4 burning (save ends)
      - effect: A burning creature takes 1d6 fire damage at the start of each of their
          turns. A burning object takes 1d6 fire damage at the end of each
          round.
        name: Effect
  - name: Caldera
    icon: ❇️
    cost: 5 Malice
    keywords:
      - Area
    type: Main action
    distance: Special
    target: Each enemy and object in the area
    effects:
      - roll: Power Roll + 4
        t1: The distance is a 2 burst; 8 fire damage; M < 2 pull 2
        t2: The distance is a 3 burst; 12 fire damage; M < 3 pull 4
        t3: The distance is a 4 burst; 15 fire damage; M < 4 pull 6
      - effect: The outermost squares of the area become a 1-square-tall wall of stone.
          The rest of the area is on fire until the end of the encounter. A
          creature who enters the area for the first time in a round or starts
          their turn there takes 3 fire damage.
        name: Effect
  - name: Blazing Leap
    icon: 👤
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The red fist jumps up to 5 squares. Each creature adjacent to them when
          they land takes 5 fire damage.
        name: Effect
  - name: Heat and Pressure
    icon: ❗️
    keywords:
      - Melee
    type: Free triggered action
    distance: Melee 3
    target: The triggering creature
    trigger: A creature within distance willingly moves or shifts away from the red
      fist.
    effects:
      - name: Effect
        effect: The target makes a **Might test**. A target with fire immunity
          automatically obtains a tier 3 outcome.
        t1: Weakened and slowed (save ends)
        t2: Weakened (EoT)
        t3: No effect
  - name: Guardian Block
    icon: ❗️
    keywords:
      - Melee
    type: Triggered action
    distance: Melee 3
    target: Self
    trigger: An ally within distance is targeted by an enemy's ability.
    effects:
      - effect: The red fist becomes the target of the triggering ability, then can make
          a free strike against the enemy after the ability resolves.
        name: Effect
```