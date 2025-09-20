---
agility: 3
ancestry:
- Draconian
- Dragon
- Humanoid
ev: '32'
file_basename: Lydixavus the Deadeye
file_dpath: Monsters/Draconians/Statblocks
free_strike: 7
intuition: 3
item_id: lydixavus-the-deadeye
item_index: '106'
item_name: Lydixavus the Deadeye
level: 6
might: -1
presence: 1
reason: 3
roles:
- Elite Artillery
scc:
- mcdm.monsters.v1:monster:lydixavus-the-deadeye
scdc:
- 1.1.1:2:106
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '140'
type: monster
---

~~~ds-statblock
type: statblock
name: Lydixavus the Deadeye
level: 6
roles:
  - Elite Artillery
ancestry:
  - Draconian
  - Dragon
  - Humanoid
ev: "32"
stamina: "140"
immunities:
  - Cold 6
speed: 5
movement: Fly
size: 1M
stability: 2
free_strike: 7
might: -1
agility: 3
reason: 3
intuition: 3
presence: 1
features:
  - type: feature
    feature_type: ability
    name: Breathsnipe
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    usage: Main action
    distance: Ranged 15
    target: One enemy
    effects:
      - roll: Power Roll + 3
        tier1: 10 cold damage
        tier2: 16 cold damage; the target takes a bane on their next strike
        tier3: 19 cold damage; the target has a double bane on their next strike
  - type: feature
    feature_type: ability
    name: Ice Lob
    icon: 🔳
    keywords:
      - Area
      - Magic
      - Ranged
    usage: Main action
    distance: 2 cube within 10
    target: Each enemy and object in the area
    effects:
      - roll: Power Roll + 3
        tier1: 7 cold damage; M < 1 dazed (save ends)
        tier2: 12 cold damage; M < 2 dazed (save ends)
        tier3: 15 cold damage; M < 3 dazed (save ends)
  - type: feature
    feature_type: ability
    name: Parting Gift
    icon: 👤
    keywords:
      - "-"
    usage: Maneuver
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: Lydixavus flies up to their speed, leaving a size 1S ice mine in the
          space they took off from. The ice mine explodes when an enemy enters
          its space, using the power roll for the Ice Lob ability, and targeting
          the triggering creature and each creature and object adjacent to the
          ice mine.
  - type: feature
    feature_type: ability
    name: Wasn't Aiming For You
    icon: ❗️
    keywords:
      - "-"
    usage: Triggered action
    distance: Self
    target: Self
    trigger: Lydixavus obtains a tier 1 outcome on their signature ability.
    effects:
      - name: Effect
        effect: Lydixavus uses their signature ability again, targeting a creature
          within 5 squares of the original target.
  - type: feature
    feature_type: trait
    name: Scorekeeping Scales
    icon: ⭐️
    effects:
      - effect: Lydixavus knows the location of every creature who has ever dealt damage
          to them. If any of those creatures are within 20 squares of Lydixavus,
          Lydixavus always has line of effect to them as long as a size 1
          opening exists between Lydixavus and the target.
~~~