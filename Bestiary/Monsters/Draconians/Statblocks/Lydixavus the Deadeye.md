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

```ds-statblock
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
traits:
  - name: Scorekeeping Scales
    effects:
      - effect: Lydixavus knows the location of every creature who has ever dealt damage
          to them. If any of those creatures are within 20 squares of Lydixavus,
          Lydixavus always has line of effect to them as long as a size 1
          opening exists between Lydixavus and the target.
abilities:
  - name: Breathsnipe
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 15
    target: One enemy
    effects:
      - roll: Power Roll + 3
        t1: 10 cold damage
        t2: 16 cold damage; the target takes a bane on their next strike
        t3: 19 cold damage; the target has a double bane on their next strike
  - name: Ice Lob
    icon: 🔳
    keywords:
      - Area
      - Magic
      - Ranged
    type: Main action
    distance: 2 cube within 10
    target: Each enemy and object in the area
    effects:
      - roll: Power Roll + 3
        t1: 7 cold damage; M < 1 dazed (save ends)
        t2: 12 cold damage; M < 2 dazed (save ends)
        t3: 15 cold damage; M < 3 dazed (save ends)
  - name: Parting Gift
    icon: 👤
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: Lydixavus flies up to their speed, leaving a size 1S ice mine in the
          space they took off from. The ice mine explodes when an enemy enters
          its space, using the power roll for the Ice Lob ability, and targeting
          the triggering creature and each creature and object adjacent to the
          ice mine.
        name: Effect
  - name: Wasn't Aiming For You
    icon: ❗️
    keywords:
      - "-"
    type: Triggered action
    distance: Self
    target: Self
    trigger: Lydixavus obtains a tier 1 outcome on their signature ability.
    effects:
      - effect: Lydixavus uses their signature ability again, targeting a creature
          within 5 squares of the original target.
        name: Effect
```