---
agility: 0
ancestry:
- Humanoid
- Rival
ev: '48'
file_basename: Rival Talent
file_dpath: Monsters/Rivals/4th Echelon/Statblocks
free_strike: 10
intuition: 0
item_id: rival-talent
item_index: '32'
item_name: Rival Talent
level: 10
might: 0
presence: 1
reason: 5
roles:
- Elite Hexer
scc:
- mcdm.monsters.v1:monster:rival-talent
scdc:
- 1.1.1:2:32
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '220'
type: monster
---

```ds-statblock
name: Rival Talent
level: 10
roles:
  - Elite Hexer
ancestry:
  - Humanoid
  - Rival
ev: "48"
stamina: "220"
speed: 5
size: 1M
stability: 2
free_strike: 10
might: 0
agility: 0
reason: 5
intuition: 0
presence: 1
traits:
  - name: Rivalry
    effects:
      - effect: At the start of an encounter, the talent chooses one creature within
          their line of effect. Both the talent and the creature can add a d3
          roll to power rolls they make against each other.
abilities:
  - name: Override
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Psionic
      - Ranged
      - Strike
      - Telekinesis
    type: Main action
    distance: Ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 5
        t1: 15 psychic damage
        t2: 20 psychic damage
        t3: 24 psychic damage
      - effect: Each target moves up to their speed and can make a free strike against
          one enemy of the talent's choice. The target's movement can provoke
          opportunity attacks, but they can't otherwise be moved in a way that
          would harm them.
        cost: 4 Malice
  - name: Steal Time
    icon: 🏹
    cost: 3 Malice
    keywords:
      - Chronopathy
      - Psionic
      - Ranged
    type: Maneuver
    distance: Ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 5
        t1: R < 3 slowed (save ends)
        t2: R < 4 restrained (save ends)
        t3: R < 5 restrained (save ends)
      - effect: \*\*Effect:\*\*One ally within distance can use an additional main
          action on their next turn.
  - name: Psionic Retribution
    icon: ❗️
    cost: 2 Malice
    keywords:
      - Psionic
    type: Triggered action
    distance: Self; see below
    target: Self
    trigger: A creature deals damage to the talent.
    effects:
      - effect: The talent halves the damage and shifts up to 2 squares. The triggering
          creature takes psychic damage equal to half the damage dealt and is
          pushed up to 5 squares.
        name: Effect
```