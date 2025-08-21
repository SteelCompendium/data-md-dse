---
agility: -1
ancestry:
- Frost Giant
- Giant
ev: '40'
file_basename: Frost Giant Storm Hurler
file_dpath: Monsters/Giants/Statblocks
free_strike: 9
intuition: 0
item_id: frost-giant-storm-hurler
item_index: '200'
item_name: Frost Giant Storm Hurler
level: 8
might: 4
presence: 0
reason: 0
roles:
- Elite Artillery
scc:
- mcdm.monsters.v1:monster:frost-giant-storm-hurler
scdc:
- 1.1.1:2:200
size: '4'
source: mcdm.monsters.v1
speed: 7
stability: 5
stamina: '180'
type: monster
---

```ds-statblock
name: Frost Giant Storm Hurler
level: 8
roles:
  - Elite Artillery
ancestry:
  - Frost Giant
  - Giant
ev: "40"
stamina: "180"
immunities:
  - Cold 8
speed: 7
size: "4"
stability: 5
free_strike: 9
might: 4
agility: -1
reason: 0
intuition: 0
presence: 0
traits:
  - name: Kingdom of Isolation
    effects:
      - effect: The storm hurler is surrounded by a snowstorm. Any enemy who starts
          their turn within 2 squares of the storm hurler can't shift.
abilities:
  - name: Ice Javelins
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 15
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        t1: 13 cold damage
        t2: 18 cold damage; M < 3 bleeding (save ends)
        t3: 22 cold damage; M < 4 bleeding (save ends)
      - effect: Whenever a creature bleeding this way takes damage from that condition,
          their speed decreases by 1 (to a minimum of 0) until that condition
          ends.
        name: Effect
  - name: Flower of Frost
    cost: 3 Malice
    keywords:
      - Magic
      - Ranged
    type: Main action
    distance: Ranged 15
    target: Special
    effects:
      - name: Effect
        effect: The storm hurler throws three size 1L ice javelins into unoccupied
          squares within distance. Each javelin has 30 Stamina and fire weakness
          5. At the start of the storm hurler's next turn, all javelins not
          destroyed explode in a shower of icicles. Each enemy and object within
          3 squares of an exploding javelin makes an **Agility test**.
        t1: 14 cold damage; push 4; bleeding (save ends)
        t2: 11 cold damage; push 2; slowed (save ends)
        t3: 7 cold damage
  - name: Ice Dance
    keywords:
      - Melee
    type: Maneuver
    distance: Melee 1
    target: One giant ally
    effects:
      - effect: The storm hurler and the target each shift up to 6 squares while staying
          adjacent to each other. The target can then jump up to 5 squares and
          make a free strike.
        name: Effect
  - name: Frozen Retribution
    keywords:
      - "-"
    type: Triggered action
    distance: Self
    target: Self
    trigger: The storm hurler is targeted by a ranged strike.
    effects:
      - effect: The triggering strike has a double bane. If the strike obtains a tier 1
          outcome, the storm hurler uses Ice Javelins against the creature who
          made it.
        name: Effect
```