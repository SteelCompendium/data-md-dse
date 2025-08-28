---
agility: 0
ancestry:
- Humanoid
- Orc
ev: '6'
file_basename: Orc Godcaller
file_dpath: Monsters/Orcs/Statblocks
free_strike: 3
intuition: 1
item_id: orc-godcaller
item_index: '127'
item_name: Orc Godcaller
level: 1
might: 1
presence: 2
reason: 0
roles:
- Platoon Support
scc:
- mcdm.monsters.v1:monster:orc-godcaller
scdc:
- 1.1.1:2:127
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 0
stamina: '30'
type: monster
---

```ds-statblock
name: Orc Godcaller
level: 1
roles:
  - Platoon Support
ancestry:
  - Humanoid
  - Orc
ev: "6"
stamina: "30"
speed: 6
size: 1M
stability: 0
free_strike: 3
might: 1
agility: 0
reason: 0
intuition: 1
presence: 2
traits:
  - name: Relentless
    effects:
      - effect: If the godcaller is reduced to 0 Stamina, they can make a free strike
          before dying. If the target of the free strike is reduced to 0
          Stamina, the godcaller is reduced to 1 Stamina instead.
abilities:
  - name: Power Chord
    icon: ⚔️
    cost: Signature Ability
    keywords:
      - Magic
      - Melee
      - Ranged
      - Strike
    type: Main action
    distance: Melee 1 or ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 5 sonic damage
        t2: 7 sonic damage
        t3: 9 sonic damage; P < 2 weakened (save ends)
  - name: Cadenza
    icon: 🏹
    keywords:
      - Magic
      - Ranged
    type: Main action
    distance: Ranged 10
    target: One ally
    effects:
      - effect: The target moves up to their speed and can use a main action.
        name: Effect
      - effect: The godcaller targets a second ally.
        cost: 3 Malice
  - name: Rallying Ostinato
    icon: 🏹
    cost: 2 Malice
    keywords:
      - Magic
      - Ranged
    type: Maneuver
    distance: Ranged 10
    target: Self and three allies
    effects:
      - effect: Each target regains 15 Stamina and ignores difficult terrain until the
          end of the encounter.
        name: Effect
```