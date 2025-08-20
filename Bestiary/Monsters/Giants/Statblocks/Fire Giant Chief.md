---
agility: 3
ancestry:
- Fire Giant
- Giant
ev: '44'
file_basename: Fire Giant Chief
file_dpath: Monsters/Giants/Statblocks
free_strike: 9
intuition: 2
item_id: fire-giant-chief
item_index: '192'
item_name: Fire Giant Chief
level: 9
might: 5
presence: 3
reason: 0
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:fire-giant-chief
scdc:
- 1.1.1:2:192
size: '5'
source: mcdm.monsters.v1
speed: 10
stability: 10
stamina: '240'
type: monster
---

```ds-statblock
name: Fire Giant Chief
level: 9
roles:
  - Leader
ancestry:
  - Fire Giant
  - Giant
ev: "44"
stamina: "240"
immunities:
  - Fire 10
speed: 10
size: "5"
stability: 10
free_strike: 9
might: 5
agility: 3
reason: 0
intuition: 2
presence: 3
traits:
  - name: Scorching Skin
    effects:
      - effect: Whenever an adjacent enemy grabs the chief or uses a melee ability
          against them, that enemy takes 9 fire damage, and if they have M < 4
          they are weakened (save ends)
abilities:
  - name: Roiling Fist
    cost: Signature Ability
    keywords:
      - Area
      - Ranged
      - Weapon
    type: Main action
    distance: 3 cube within 4
    target: Each enemy and object in the area
    effects:
      - effect: |-
          Each target makes either an **Agility test** or an **Intuition test**.
          - **≤11:** 18 fire damage; prone; weakened (save ends)
          - **12-16:** 14 fire damage; prone
          - **17+:** 9 fire damage
  - name: Burning Kick
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 4
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 5
        t1: 14 damage; push 5; A < 3, 9 fire damage
        t2: 19 damage; push 10; A < 4, 9 fire damage
        t3: 23 damage; push 15; A < 5, 9 fire damage
  - name: Lava Pillar
    cost: 3 Malice
    keywords:
      - Area
      - Ranged
    type: Maneuver
    distance: 3 cube within 10
    target: Each enemy and object in the area
    effects:
      - roll: Power Roll + 5
        t1: 5 fire damage; M < 3, vertical push 3
        t2: 7 fire damage; M < 4, vertical push 4
        t3: 9 fire damage; M < 5, vertical push 5
  - name: Fuel the Fire
    cost: 1 Malice
    keywords:
      - Ranged
    type: Triggered action
    distance: Ranged 12
    target: The triggering ally
    trigger: A fire giant ally within distance makes a strike.
    effects:
      - effect: The strike has a double edge and deals an extra 10 fire damage.
  - name: Forward!
    cost: Villain Action 1
    keywords:
      - Area
    type: "-"
    distance: 10 burst
    target: Self and each ally in the area
    effects:
      - effect: Each target shifts up to their speed and can make a free strike. Any
          enemy who takes damage from a free strike this way and who has A < 4
          is burning (save ends). A burning enemy takes 1d6 fire damage at the
          start of each of their turns.
  - name: Burning Legion
    cost: Villain Action 2
    keywords:
      - Ranged
    type: "-"
    distance: Ranged 15
    target: Special
    effects:
      - effect: The chief shifts up to 10 squares. Five fire giant fireballer then
          arrive in unoccupied spaces within distance.
  - name: All to Cinders
    cost: Villain Action 3
    keywords:
      - Area
    type: "-"
    distance: 10 burst
    target: Self and each fire giant ally in the are
    effects:
      - effect: >-
          Each target unleashes a wave of fire, and each enemy within 2 squares
          of any target makes an Agility test. An enemy affected by two targets
          takes a bane on the test, while an enemy affected by three or more
          targets has a double bane.

          - **≤11:** 18 fire damage

          - **12-16:** 14 fire damage

          - **17+:** 9 fire damage
```