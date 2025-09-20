---
agility: 2
ancestry:
- Humanoid
- Time Raider
ev: '10'
file_basename: Time Raider Cannonfall
file_dpath: Monsters/Time Raiders/Statblocks
free_strike: 5
intuition: 2
item_id: time-raider-cannonfall
item_index: '147'
item_name: Time Raider Cannonfall
level: 3
might: 0
presence: 0
reason: 2
roles:
- Platoon Artillery
scc:
- mcdm.monsters.v1:monster:time-raider-cannonfall
scdc:
- 1.1.1:2:147
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 3
stamina: '40'
type: monster
---

~~~ds-statblock
type: statblock
name: Time Raider Cannonfall
level: 3
roles:
  - Platoon Artillery
ancestry:
  - Humanoid
  - Time Raider
ev: "10"
stamina: "40"
immunities:
  - Psychic 3
speed: 5
size: 1L
stability: 3
free_strike: 5
might: 0
agility: 2
reason: 2
intuition: 2
presence: 0
features:
  - type: feature
    feature_type: ability
    name: Sunderbuss
    icon: 🔳
    ability_type: Signature Ability
    keywords:
      - Area
      - Psionic
      - Ranged
      - Weapon
    usage: Main action
    distance: 3 cube within 10
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        tier1: 4 sonic damage
        tier2: 7 sonic damage
        tier3: 10 sonic damage; prone; M < 2 slowed (save ends)
      - name: Effect
        effect: A layer of ground beneath the area that is 1 square deep is destroyed.
  - type: feature
    feature_type: ability
    name: Buss Buffe
    icon: ❗️
    cost: 1 Malice
    keywords:
      - Area
      - Psionic
    usage: Free triggered action
    distance: 5 burst
    target: Self and each ally in the area
    trigger: A creature damages the cannonfall with a ranged or area ability.
    effects:
      - name: Effect
        effect: The damage is halved for the cannonfall and each target also affected by
          the triggering ability
  - type: feature
    feature_type: trait
    name: Foresight Squared
    icon: ⭐️
    effects:
      - effect: The cannonfall doesn't take a bane on strikes against creatures with
          concealment or cover.
~~~