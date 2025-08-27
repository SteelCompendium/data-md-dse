---
agility: 4
ancestry:
- Frost Giant
- Giant
ev: '40'
file_basename: Frost Giant Wind Sprinter
file_dpath: Monsters/Giants/Statblocks
free_strike: 8
intuition: 0
item_id: frost-giant-wind-sprinter
item_index: '202'
item_name: Frost Giant Wind Sprinter
level: 8
might: 4
presence: 0
reason: -1
roles:
- Elite Harrier
scc:
- mcdm.monsters.v1:monster:frost-giant-wind-sprinter
scdc:
- 1.1.1:2:202
size: '4'
source: mcdm.monsters.v1
speed: 10
stability: 5
stamina: '200'
type: monster
---

```ds-statblock
name: Frost Giant Wind Sprinter
level: 8
roles:
  - Elite Harrier
ancestry:
  - Frost Giant
  - Giant
ev: "40"
stamina: "200"
immunities:
  - Cold 8
speed: 10
size: "4"
stability: 5
free_strike: 8
might: 4
agility: 4
reason: -1
intuition: 0
presence: 0
traits:
  - name: Crush Underfoot
    effects:
      - effect: The wind sprinter can move through enemies' spaces at their usual speed.
          The first time on a turn that a wind sprinter enters a creature's
          space, that creature can choose to fall prone or to take 8 damage.
  - name: Kingdom of Isolation
    effects:
      - effect: The wind sprinter is surrounded by a snowstorm. Any enemy who starts
          their turn within 2 squares of the wind sprinter can't shift.
abilities:
  - name: Cold Axe
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 3
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        t1: 12 damage
        t2: 17 damage; A < 3 bleeding (save ends)
        t3: 21 damage; A < 4 bleeding (save ends)
      - effect: A target who is already bleeding takes an extra 1d6 cold damage.
        name: Effect
  - name: Blizzard Surge
    icon: 👤
    cost: 5 Malice
    keywords:
      - "-"
    type: Main action
    distance: Self
    target: Self
    effects:
      - effect: The wind sprinter shifts up to their speed and uses Cold Axe against
          each enemy who comes within 2 squares of them during the move. The
          wind sprinter makes one power roll against all targets.
        name: Effect
  - name: Ice Dance
    icon: 🗡
    keywords:
      - Melee
    type: Maneuver
    distance: Melee 1
    target: One giant ally
    effects:
      - effect: The wind sprinter and the target each shift up to 6 squares while
          staying adjacent to each other. The target can then jump up to 5
          squares and make a free strike.
        name: Effect
  - name: Begone, Smallfolk!
    icon: ❗️
    keywords:
      - "-"
    type: Triggered action
    distance: Self
    target: Self
    trigger: The wind sprinter takes damage.
    effects:
      - effect: The wind sprinter moves up to their speed and uses Cold Axe against one
          target.
        name: Effect
```