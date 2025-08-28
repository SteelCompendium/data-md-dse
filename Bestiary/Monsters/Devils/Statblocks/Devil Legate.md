---
agility: 1
ancestry:
- Devil
- Infernal
ev: '28'
file_basename: Devil Legate
file_dpath: Monsters/Devils/Statblocks
free_strike: 6
intuition: 1
item_id: devil-legate
item_index: '303'
item_name: Devil Legate
level: 5
might: 3
presence: 2
reason: 0
roles:
- Elite Defender
scc:
- mcdm.monsters.v1:monster:devil-legate
scdc:
- 1.1.1:2:303
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 2
stamina: '160'
type: monster
---

~~~ds-statblock
name: Devil Legate
level: 5
roles:
  - Elite Defender
ancestry:
  - Devil
  - Infernal
ev: "28"
stamina: "160"
immunities:
  - Fire 5
speed: 6
size: 1M
stability: 2
free_strike: 6
might: 3
agility: 1
reason: 0
intuition: 1
presence: 2
traits:
  - name: Hellish Bailiff
    effects:
      - effect: The legate has damage immunity 3 while in one of the Seven Cities of
          Hell or within 10 squares of a non-minion devil who is of a higher
          level than them.
  - name: True Name
    effects:
      - effect: If a creature within 10 squares speaks the legate's true name, the
          legate loses their damage immunities, any nondamaging effects of their
          signature ability, and their Devilish Charm ability until the end of
          the encounter.
abilities:
  - name: Infernal Pike
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        t1: 9 damage
        t2: 14 damage; A < 2 slowed (save ends)
        t3: \*\*17 damage; A < 3 slowed (save ends)
      - effect: If the targets are adjacent to each other, this ability deals an extra 3
          damage.
        name: Effect
  - name: Writ of Execution
    icon: 🗡
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - effect: "**Power Roll + 3**"
        t1: 6 damage; M < 1 prone
        t2: 11 damage; M < 2 prone and can't stand (save ends)
        t3: \*\*14 damage; M < 3 prone and can't stand (save ends)
      - effect: If this ability is used as part of the Charge main action, the legate
          ignores difficult terrain during the charge. Each creature and object
          whose space the legate moves through takes the damage from this
          ability, but not its additional effects.
        name: Effect
  - name: Law and Order
    icon: 🗡
    keywords:
      - Melee
    type: Maneuver
    distance: Melee 1
    target: One creature
    effects:
      - effect: The target is taunted by the legate (save ends). The legate can have
          only one creature taunted at a time.
        name: Effect
  - name: Devilish Charm
    icon: ❗️
    cost: 2 Malice
    keywords:
      - Magic
      - Ranged
    type: Triggered action
    distance: Ranged 5
    target: The triggering creature
    trigger: A creature targets the legate with a strike.
    effects:
      - name: Effect
        effect: The target makes a Presence test
        t1: The legate chooses a new target for the strike.
        t2: The legate halves the triggering damage.
        t3: The target takes a bane on the strike.
~~~