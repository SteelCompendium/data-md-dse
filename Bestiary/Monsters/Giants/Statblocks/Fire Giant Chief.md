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

~~~ds-statblock
type: statblock
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
features:
  - type: feature
    feature_type: ability
    name: Roiling Fist
    icon: 🔳
    ability_type: Signature Ability
    keywords:
      - Area
      - Ranged
      - Weapon
    usage: Main action
    distance: 3 cube within 4
    target: Each enemy and object in the area
    effects:
      - name: Effect
        effect: Each target makes either an **Agility test** or an **Intuition test**.
        tier1: 18 fire damage; prone; weakened (save ends)
        tier2: 14 fire damage; prone
        tier3: 9 fire damage
  - type: feature
    feature_type: ability
    name: Burning Kick
    icon: 🗡
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    usage: Main action
    distance: Melee 4
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 5
        tier1: 14 damage; push 5; A < 3 9 fire damage
        tier2: 19 damage; push 10; A < 4 9 fire damage
        tier3: 23 damage; push 15; A < 5 9 fire damage
  - type: feature
    feature_type: ability
    name: Lava Pillar
    icon: 🔳
    cost: 3 Malice
    keywords:
      - Area
      - Ranged
    usage: Maneuver
    distance: 3 cube within 10
    target: Each enemy and object in the area
    effects:
      - roll: Power Roll + 5
        tier1: 5 fire damage; M < 3 vertical push 3
        tier2: 7 fire damage; M < 4 vertical push 4
        tier3: 9 fire damage; M < 5 vertical push 5
  - type: feature
    feature_type: ability
    name: Fuel the Fire
    icon: ❗️
    cost: 1 Malice
    keywords:
      - Ranged
    usage: Triggered action
    distance: Ranged 12
    target: The triggering ally
    trigger: A fire giant ally within distance makes a strike.
    effects:
      - name: Effect
        effect: The strike has a double edge and deals an extra 10 fire damage.
  - type: feature
    feature_type: ability
    name: Forward!
    icon: ☠️
    ability_type: Villain Action 1
    keywords:
      - Area
    usage: "-"
    distance: 10 burst
    target: Self and each ally in the area
    effects:
      - name: Effect
        effect: Each target shifts up to their speed and can make a free strike. Any
          enemy who takes damage from a free strike this way and who has A < 4
          is burning (save ends). A burning enemy takes 1d6 fire damage at the
          start of each of their turns.
  - type: feature
    feature_type: ability
    name: Burning Legion
    icon: ☠️
    ability_type: Villain Action 2
    keywords:
      - Ranged
    usage: "-"
    distance: Ranged 15
    target: Special
    effects:
      - name: Effect
        effect: The chief shifts up to 10 squares. Five fire giant fireballer then
          arrive in unoccupied spaces within distance.
  - type: feature
    feature_type: ability
    name: All to Cinders
    icon: ☠️
    ability_type: Villain Action 3
    keywords:
      - Area
    usage: "-"
    distance: 10 burst
    target: Self and each fire giant ally in the area
    effects:
      - name: Effect
        effect: Each target unleashes a wave of fire, and each enemy within 2 squares of
          any target makes an Agility test. An enemy affected by two targets
          takes a bane on the test, while an enemy affected by three or more
          targets has a double bane.
        tier1: 18 fire damage
        tier2: 14 fire damage
        tier3: 9 fire damage
  - type: feature
    feature_type: trait
    name: Scorching Skin
    icon: ⭐️
    effects:
      - effect: Whenever an adjacent enemy grabs the chief or uses a melee ability
          against them, that enemy takes 9 fire damage, and if they have M < 4
          they are weakened (save ends)
~~~