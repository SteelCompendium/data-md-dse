---
agility: 0
ancestry:
- Humanoid
- Rival
ev: '28'
file_basename: Rival Talent
file_dpath: Monsters/Rivals/2nd Echelon/Statblocks
free_strike: 6
intuition: 0
item_id: rival-talent
item_index: '18'
item_name: Rival Talent
level: 5
might: 0
presence: 1
reason: 3
roles:
- Elite Hexer
scc:
- mcdm.monsters.v1:monster:rival-talent
scdc:
- 1.1.1:2:18
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '120'
type: monster
---

~~~ds-statblock
name: Rival Talent
level: 5
roles:
  - Elite Hexer
ancestry:
  - Humanoid
  - Rival
ev: "28"
stamina: "120"
speed: 5
size: 1M
stability: 2
free_strike: 6
might: 0
agility: 0
reason: 3
intuition: 0
presence: 1
traits:
  - name: Rivalry
    effects:
      - effect: At the start of an encounter, the talent chooses one creature within
          their line of effect. Both the talent and the creature can add a d3
          roll to power rolls they make against each other.
abilities:
  - name: Overwhelming Rend
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
      - roll: Power Roll + 3
        t1: 9 psychic damage; push 2; M < 1 prone
        t2: 14 psychic damage; push 3; M < 2 prone
        t3: 17 psychic damage; push 4; M < 3 prone
  - name: Disarrange Thoughts
    icon: 🏹
    cost: 2 Malice
    keywords:
      - Psionic
      - Ranged
      - Telepathy
    type: Maneuver
    distance: Ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        t1: 6 psychic damage; R < 1 dazed (save ends)
        t2: 6 psychic damage; R < 2 dazed (save ends)
        t3: 6 psychic damage; R < 3 dazed and slowed (save ends)
  - name: Precognitive Shift
    icon: ❗️
    cost: 1 Malice
    keywords:
      - Psionic
    type: Triggered action
    distance: Self
    target: Self
    trigger: A creature deals damage to the talent.
    effects:
      - effect: The talent halves the damage and shifts up to 2 squares
        name: Effect
~~~