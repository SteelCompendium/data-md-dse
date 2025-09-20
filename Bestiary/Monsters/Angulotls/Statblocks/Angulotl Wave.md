---
agility: 0
ancestry:
- Angulotl
- Humanoid
ev: '3'
file_basename: Angulotl Wave
file_dpath: Monsters/Angulotls/Statblocks
free_strike: 1
intuition: 2
item_id: angulotl-wave
item_index: '241'
item_name: Angulotl Wave
level: 1
might: 0
presence: 2
reason: 0
roles:
- Horde Controller
scc:
- mcdm.monsters.v1:monster:angulotl-wave
scdc:
- 1.1.1:2:241
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '10'
type: monster
---

~~~ds-statblock
type: statblock
name: Angulotl Wave
level: 1
roles:
  - Horde Controller
ancestry:
  - Angulotl
  - Humanoid
ev: "3"
stamina: "10"
immunities:
  - Poison 2
speed: 5
movement: Climb, swim
size: 1S
stability: 0
free_strike: 1
might: 0
agility: 0
reason: 0
intuition: 2
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Refulgent Beams
    icon: 🏹
    ability_type: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    usage: Main action
    distance: Ranged 8
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        tier1: 3 holy damage
        tier2: 4 holy damage; R < 1 the target is illuminated (save ends)
        tier3: 5 holy damage; R < 2 the target is illuminated (save ends)
      - name: Effect
        effect: An illuminated creature or object can't hide or become invisible, and
          any strike made against an illuminated target gains an edge.
  - type: feature
    feature_type: ability
    name: Noxious Bubble
    icon: 🔳
    cost: 2 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    usage: Main action
    distance: 2 cube of unoccupied space within 10
    target: Special
    effects:
      - name: Effect
        effect: A bubble of toxic gas fills the area, ready to pop. If any creature or
          object touches the bubble or if the bubble takes damage, it bursts.
          Each angulotl adjacent to the bubble is wet until the end of the
          encounter, and each enemy adjacent to the bubble makes a **Might
          test**.
        tier1: 3 poison damage; the target is wet and weakened (save ends)
        tier2: 2 poison damage; the target is wet (save ends)
        tier3: 1 poison damage; the target is wet (EoT)
  - type: feature
    feature_type: trait
    name: Toxiferous
    icon: ⭐️
    effects:
      - effect: Whenever an adjacent enemy grabs the wave or uses a melee ability
          against them, that enemy takes 2 poison damage.
~~~