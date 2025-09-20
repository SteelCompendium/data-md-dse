---
agility: 2
ancestry:
- Fire Giant
- Giant
ev: '44'
file_basename: Fire Giant Lightbearer
file_dpath: Monsters/Giants/Statblocks
free_strike: 9
intuition: 4
item_id: fire-giant-lightbearer
item_index: '193'
item_name: Fire Giant Lightbearer
level: 9
might: 4
presence: 1
reason: 0
roles:
- Elite Support
scc:
- mcdm.monsters.v1:monster:fire-giant-lightbearer
scdc:
- 1.1.1:2:193
size: '4'
source: mcdm.monsters.v1
speed: 8
stability: 5
stamina: '200'
type: monster
---

~~~ds-statblock
type: statblock
name: Fire Giant Lightbearer
level: 9
roles:
  - Elite Support
ancestry:
  - Fire Giant
  - Giant
ev: "44"
stamina: "200"
immunities:
  - Fire 9
speed: 8
size: "4"
stability: 5
free_strike: 9
might: 4
agility: 2
reason: 0
intuition: 4
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Flamelash
    icon: 🗡
    ability_type: Signature Ability
    keywords:
      - Magic
      - Melee
      - Strike
    usage: Main action
    distance: Melee 6
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        tier1: 13 fire damage; slide 2
        tier2: 17 fire damage; slide 4
        tier3: 22 fire damage; slide 6
  - type: feature
    feature_type: ability
    name: Living Blaze
    icon: 🏹
    cost: 3 Malice
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 6
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        tier1: 15 fire damage
        tier2: 21 fire damage
        tier3: 26 fire damage
      - name: Effect
        effect: The blaze ricochets, targeting one additional target within 4 squares of
          an original target and taking a bane against that target, or targeting
          two additional targets within 2 squares of an original target and
          having a double bane against those targets. The lightbearer makes one
          power roll against all targets.
  - type: feature
    feature_type: ability
    name: Travel By Fire
    icon: 🏹
    keywords:
      - Magic
      - Ranged
    usage: Maneuver
    distance: Ranged 5
    target: Two creatures or objects
    effects:
      - name: Effect
        effect: The lightbearer can target themself with this ability. Each target takes
          1d6 fire damage and teleports in a plume of smoke to swap places with
          the other target.
  - type: feature
    feature_type: ability
    name: Emergency Beacon
    icon: ❗️
    keywords:
      - "-"
    usage: Triggered action
    distance: Self
    target: Self
    trigger: The lightbearer takes damage.
    effects:
      - name: Effect
        effect: The lightbearer emits a beacon of light until the start of their next
          turn. Each fire giant who has line of effect to the lightbearer has a
          double edge on abilities.
  - type: feature
    feature_type: trait
    name: Healing Heat
    icon: ⭐️
    effects:
      - effect: Any fire giant targeted by the lightbearer's damage-dealing abilities
          ignores the damage and instead regains Stamina equal to the damage
          that would have been dealt. If the lightbearer moves a fire giant
          using an ability, they can choose to ignore stability.
  - type: feature
    feature_type: trait
    name: Searing Skin
    icon: ⭐️
    effects:
      - effect: Whenever an adjacent enemy grabs the lightbearer or uses a melee ability
          against them, that enemy takes 5 fire damage.
~~~