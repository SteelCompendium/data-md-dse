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
traits:
  - name: Toxiferous
    effects:
      - effect: Whenever an adjacent enemy grabs the wave or uses a melee ability
          against them, that enemy takes 2 poison damage.
abilities:
  - name: Refulgent Beams
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 8
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        t1: 3 holy damage
        t2: 4 holy damage; R < 1 the target is illuminated (save ends)
        t3: 5 holy damage; R < 2 the target is illuminated (save ends)
      - effect: An illuminated creature or object can't hide or become invisible, and
          any strike made against an illuminated target gains an edge.
        name: Effect
  - name: Noxious Bubble
    icon: 🔳
    cost: 2 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    type: Main action
    distance: 2 cube of unoccupied space within 10
    target: Special
    effects:
      - name: Effect
        effect: A bubble of toxic gas fills the area, ready to pop. If any creature or
          object touches the bubble or if the bubble takes damage, it bursts.
          Each angulotl adjacent to the bubble is wet until the end of the
          encounter, and each enemy adjacent to the bubble makes a **Might
          test**.
        t1: 3 poison damage; the target is wet and weakened (save ends)
        t2: 2 poison damage; the target is wet (save ends)
        t3: 1 poison damage; the target is wet (EoT)
~~~