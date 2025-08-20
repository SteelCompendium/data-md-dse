---
agility: 0
ancestry:
- Humanoid
- Rival
ev: '16'
file_basename: Rival Talent
file_dpath: Monsters/Rivals/1st Echelon/Statblocks
free_strike: 5
intuition: 0
item_id: rival-talent
item_index: '11'
item_name: Rival Talent
level: 2
might: 0
presence: 1
reason: 2
roles:
- Elite Hexer
scc:
- mcdm.monsters.v1:monster:rival-talent
scdc:
- 1.1.1:2:11
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '60'
type: monster
---

```ds-statblock
name: Rival Talent
level: 2
roles:
  - Elite Hexer
ancestry:
  - Humanoid
  - Rival
ev: "16"
stamina: "60"
speed: 5
size: 1M
stability: 2
free_strike: 5
might: 0
agility: 0
reason: 2
intuition: 0
presence: 1
traits:
  - name: Rivalry
    effects:
      - effect: At the start of an encounter, the talent chooses one creature within
          their line of effect. Both the talent and the creature can add a d3
          roll to power rolls they make against each other.
abilities:
  - name: Reverberating Blast
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
      - roll: Power Roll + 2
        t1: 7 psychic damage; M < 0 prone
        t2: 10 psychic damage; push 2; M < 1 prone
        t3: 13 psychic damage; push 3; M < 2 prone
  - name: Muddle the Mind
    cost: 2 Malice
    keywords:
      - Psionic
      - Ranged
      - Telepathy
    type: Maneuver
    distance: Ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: R < 0 slowed (save ends)
        t2: R < 1 dazed (save ends)
        t3: R < 2 dazed and slowed (save ends)
  - name: Precognitive Shift
    cost: 1 Malice
    keywords:
      - Psionic
    type: Triggered action
    distance: Self
    target: Self
    trigger: A creature deals damage to the talent.
    effects:
      - effect: The talent halves the damage and shifts up to 2 squares
```