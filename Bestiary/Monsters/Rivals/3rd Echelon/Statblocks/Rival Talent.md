---
agility: 0
ancestry:
- Humanoid
- Rival
ev: '40'
file_basename: Rival Talent
file_dpath: Monsters/Rivals/3rd Echelon/Statblocks
free_strike: 8
intuition: 0
item_id: rival-talent
item_index: '25'
item_name: Rival Talent
level: 8
might: 0
presence: 1
reason: 4
roles:
- Elite Hexer
scc:
- mcdm.monsters.v1:monster:rival-talent
scdc:
- 1.1.1:2:25
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '180'
type: monster
---

```ds-statblock
name: Rival Talent
level: 8
roles:
  - Elite Hexer
ancestry:
  - Humanoid
  - Rival
ev: "40"
stamina: "180"
speed: 5
size: 1M
stability: 2
free_strike: 8
might: 0
agility: 0
reason: 4
intuition: 0
presence: 1
traits:
  - name: Rivalry
    effects:
      - effect: At the start of an encounter, the talent chooses one creature within
          their line of effect. Both the talent and the creature can add a d3
          roll to power rolls they make against each other.
abilities:
  - name: Control Synapses
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
      - roll: Power Roll + 4
        t1: 12 psychic damage
        t2: 17 psychic damage
        t3: 21 psychic damage
      - effect: Each target shifts up to their speed and can make a free strike against
          one enemy of the talent's choice. The target can't be moved in a way
          that would harm them.
        cost: 3 Malice
  - name: Disorientate
    cost: 2 Malice
    keywords:
      - Psionic
      - Ranged
      - Telepathy
    type: Maneuver
    distance: Ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        t1: 8 psychic damage; R < 2 dazed (save ends)
        t2: 8 psychic damage; R < 3 dazed and slowed (save ends)
        t3: 8 psychic damage; R < 4 dazed and slowed (save ends)
  - name: Mind Requital
    cost: 2 Malice
    keywords:
      - Psionic
    type: Triggered action
    distance: Self
    target: Self
    trigger: A creature deals damage to the talent.
    effects:
      - effect: The talent halves the damage and shifts up to 2 squares. The triggering
          creature takes psychic damage equal to half the damage dealt.
        name: Effect
```