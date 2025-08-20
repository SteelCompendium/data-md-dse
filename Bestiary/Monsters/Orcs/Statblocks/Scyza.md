---
agility: -1
ancestry:
- Animal
- Orc
ev: '20'
file_basename: Scyza
file_dpath: Monsters/Orcs/Statblocks
free_strike: 5
intuition: 0
item_id: scyza
item_index: '131'
item_name: Scyza
level: 3
might: 2
presence: -1
reason: -4
roles:
- Elite Mount
scc:
- mcdm.monsters.v1:monster:scyza
scdc:
- 1.1.1:2:131
size: '4'
source: mcdm.monsters.v1
speed: 6
stability: 3
stamina: '100'
type: monster
---

```ds-statblock
name: Scyza
level: 3
roles:
  - Elite Mount
ancestry:
  - Animal
  - Orc
ev: "20"
stamina: "100"
speed: 6
size: "4"
stability: 3
free_strike: 5
might: 2
agility: -1
reason: -4
intuition: 0
presence: -1
traits:
  - name: Terrible Beast
    effects:
      - effect: The scyza deals an extra 6 damage with abilities used against objects.
  - name: War Harness
    effects:
      - effect: While riding the scyza, three size 1 allies can occupy the same space.
abilities:
  - name: Clawed Kick
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        t1: 7 damage
        t2: 11 damage; prone
        t3: 14 damage; prone
      - effect: The scyza roars, and if the target has I < 2, they are frightened (save
          ends).
  - name: Whiptail
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 3
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 8 damage
        t2: 13 damage; prone
        t3: 16 damage; A < 2 bleeding (save ends)
      - effect: Against a target on top of the scyza, this ability gains an edge, and
          the target is pushed into an unoccupied adjacent square and knocked
          prone.
  - name: Crestfall
    cost: 2 Malice
    keywords:
      - Area
      - Ranged
      - Weapon
    type: Main action
    distance: 3 cube within 2
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        t1: 4 damage, 1 sonic damage; R < 0 dazed (save ends)
        t2: 7 damage, 2 sonic damage; R < 1 dazed (save ends)
        t3: 9 damage, 3 sonic damage; R < 2 dazed (save ends)
  - name: Sandstorm
    cost: 3 Malice
    keywords:
      - Area
    type: Maneuver
    distance: 3 burst
    target: Special
    effects:
      - effect: >-
          The scyza kicks up a sandstorm, granting concealment to themself and
          any ally in the area until the end of the scyza's next turn. Each
          enemy in the area makes an Intuition test.

          - **≤11:** 10 damage; prone; slowed (EoT)

          - **12-16:** 7 damage; slowed (EoT)

          - **17+:** 4 damage
  - name: Brace and Break
    keywords:
      - "-"
    type: Triggered action
    distance: Self
    target: Self
    trigger: The scyza or an ally riding the scyza is targeted by an ability.
    effects:
      - effect: Any damage dealt by the triggering ability is halved. If the creature or
          object who used the ability is within 3 squares of the scyza, the
          scyza can make a free strike against them.
```