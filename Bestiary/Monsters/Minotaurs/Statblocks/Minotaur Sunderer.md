---
agility: 1
ancestry:
- Accursed
- Humanoid
- Minotaur
ev: '20'
file_basename: Minotaur Sunderer
file_dpath: Monsters/Minotaurs/Statblocks
free_strike: 6
intuition: 2
item_id: minotaur-sunderer
item_index: '175'
item_name: Minotaur Sunderer
level: 3
might: 2
presence: -1
reason: 0
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:minotaur-sunderer
scdc:
- 1.1.1:2:175
size: '2'
source: mcdm.monsters.v1
speed: 6
stability: 2
stamina: '120'
type: monster
---

```ds-statblock
name: Minotaur Sunderer
level: 3
roles:
  - Elite Brute
ancestry:
  - Accursed
  - Humanoid
  - Minotaur
ev: "20"
stamina: "120"
speed: 6
size: "2"
stability: 2
free_strike: 6
might: 2
agility: 1
reason: 0
intuition: 2
presence: -1
traits:
  - name: Minotaur Sense
    effects:
      - effect: The sunderer can't obtain less than a tier 2 outcome when making tests
          to navigate, search, or seek.
abilities:
  - name: Spiked Maul
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
        t1: 8 damage; pull 1
        t2: 12 damage; pull 2
        t3: 15 damage; pull 3
      - effect: A target pulled adjacent to the sunderer is automatically grabbed.
        name: Effect
  - name: Fearsome Bay
    cost: 5 Malice
    keywords:
      - Area
    type: Main action
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        t1: I < 0 frightened (save ends)
        t2: I < 1 frightened (save ends)
        t3: I < 2 frightened (save ends)
      - effect: Until the end of their next turn, the minotaur has damage immunity 2 and
          deals an extra 5 damage with strikes.
        name: Effect
  - name: Disemboweling Horns
    cost: 3 Malice
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    type: Maneuver
    distance: Melee 2
    target: One creature
    effects:
      - name: Special
        effect: The target must be grabbed by the sunderer.
      - roll: Power Roll + 2
        t1: 5 damage; M < 0 bleeding (save ends)
        t2: 8 damage; M < 1 bleeding (save ends)
        t3: 9 damage; M < 2 bleeding (save ends)
      - effect: While bleeding this way, the target takes 1d6 damage at the start of
          each of their turns.
        name: Effect
  - name: Retaliatory Strike
    keywords:
      - Ranged
    type: Triggered action
    distance: Ranged 6
    target: The triggering creature
    trigger: A creature within distance deals damage to the sunderer.
    effects:
      - effect: The sunderer uses the Charge main action and Spiked Maul against the
          target.
        name: Effect
```