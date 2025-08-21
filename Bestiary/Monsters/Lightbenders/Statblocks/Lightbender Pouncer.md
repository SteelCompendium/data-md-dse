---
agility: 1
ancestry:
- Beast
- Lightbender
ev: '20'
file_basename: Lightbender Pouncer
file_dpath: Monsters/Lightbenders/Statblocks
free_strike: 5
intuition: 1
item_id: lightbender-pouncer
item_index: '207'
item_name: Lightbender Pouncer
level: 3
might: 2
presence: -1
reason: -3
roles:
- Elite Harrier
scc:
- mcdm.monsters.v1:monster:lightbender-pouncer
scdc:
- 1.1.1:2:207
size: '2'
source: mcdm.monsters.v1
speed: 1
stability: 1
stamina: '0100'
type: monster
---

```ds-statblock
name: Lightbender Pouncer
level: 3
roles:
  - Elite Harrier
ancestry:
  - Beast
  - Lightbender
ev: "20"
stamina: "0100"
speed: 1
size: "2"
stability: 1
free_strike: 5
might: 2
agility: 1
reason: -3
intuition: 1
presence: -1
traits:
  - name: Avoidance
    effects:
      - effect: Any effect on the pouncer that would be ended by a saving throw instead
          ends automatically at the end of their next turn.
abilities:
  - name: Pounce
    cost: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        t1: 7 damage
        t2: 11 damage; A < 1 prone
        t3: 14 damage; A < 2 prone
      - effect: The pouncer can make a free strike against each target they knock prone.
        name: Effect
  - name: Sparking Tail Whip
    keywords:
      - Area
      - Magic
    type: Main action
    distance: 2 burst
    target: Each enemy and object in the area
    effects:
      - roll: Power Roll + 2
        t1: 4 damage
        t2: 7 damage; A < 1 the target is dazzled (save ends)
        t3: 10 damage; A < 2 the target is dazzled (save ends)
      - effect: A dazzled target takes a bane on strikes and has line of effect only
          within 1 square.
        name: Effect
  - name: Illusory Feint
    cost: 5 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    type: Maneuver
    distance: 3 cube within 10
    target: Each enemy in the area
    effects:
      - cost: ≤11
        effect: I < 0 dazed (save ends)
        t2: I < 1 dazed (save ends)
        t3: I < 2 dazed (save ends)
      - effect: While dazed this way, a target has speed 0. If a target takes damage, or
          if someone else uses a main action to shake the target out of their
          stupor, the dazed condition ends.
        name: Effect
  - name: Striking Afterimage
    keywords:
      - Magic
    type: Triggered action
    distance: Self
    target: Self
    trigger: The pouncer takes damage from a strike.
    effects:
      - effect: The pouncer halves the damage, ignores any nondamaging effects
          associated with it, and can teleport up to 5 squares. If they teleport
          into concealment or cover, the pouncer can immediately attempt to hide
          as a free maneuver.
        name: Effect
```