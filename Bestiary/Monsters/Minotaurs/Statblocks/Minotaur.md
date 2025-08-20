---
agility: 2
ancestry:
- Accursed
- Humanoid
- Minotaur
ev: '20'
file_basename: Minotaur
file_dpath: Monsters/Minotaurs/Statblocks
free_strike: 5
intuition: 1
item_id: minotaur
item_index: '173'
item_name: Minotaur
level: 3
might: 2
presence: -1
reason: 0
roles:
- Elite Harrier
scc:
- mcdm.monsters.v1:monster:minotaur
scdc:
- 1.1.1:2:173
size: '2'
source: mcdm.monsters.v1
speed: 8
stability: 2
stamina: '100'
type: monster
---

```ds-statblock
name: Minotaur
level: 3
roles:
  - Elite Harrier
ancestry:
  - Accursed
  - Humanoid
  - Minotaur
ev: "20"
stamina: "100"
speed: 8
size: "2"
stability: 2
free_strike: 5
might: 2
agility: 2
reason: 0
intuition: 1
presence: -1
traits:
  - name: Minotaur Sense
    effects:
      - effect: The minotaur can't obtain less than a tier 2 outcome when making tests
          to navigate, search, or seek.
abilities:
  - name: Flail and Blade
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
        t1: 7 damage; push 1
        t2: 11 damage; push 2
        t3: 14 damage; push 3
      - effect: The minotaur shifts up to 3 squares
  - name: Primal Bay
    cost: 3 Malice
    keywords:
      - "-"
    type: Main action
    distance: Self
    target: Self
    effects:
      - effect: Until the end of their next turn, the minotaur has damage immunity 2 and
          deals an extra 5 damage with strikes. On their next turn, the minotaur
          can use one additional maneuver.
  - name: Goring Horns
    cost: 5 Malice
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    type: Maneuver
    distance: Melee 2
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 5 damage; I < 0 dazed (save ends)
        t2: 8 damage; I < 1 dazed (save ends)
        t3: 9 damage; I < 2 dazed (save ends)
      - effect: If this ability is used as part of the Charge main action, its potency
          increases by 1.
  - name: Retaliatory Strike
    keywords:
      - Ranged
    type: Triggered action
    distance: Ranged 8
    target: The triggering creature
    trigger: A creature within distance deals damage to the minotaur.
    effects:
      - effect: The minotaur uses theCharge main action and either Flail and Blade or
          Goring Horns against the target.
```