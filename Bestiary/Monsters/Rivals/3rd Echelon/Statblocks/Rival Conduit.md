---
agility: 0
ancestry:
- Humanoid
- Rival
ev: '40'
file_basename: Rival Conduit
file_dpath: Monsters/Rivals/3rd Echelon/Statblocks
free_strike: 8
intuition: 4
item_id: rival-conduit
item_index: '24'
item_name: Rival Conduit
level: 8
might: 3
presence: 2
reason: 1
roles:
- Elite Support
scc:
- mcdm.monsters.v1:monster:rival-conduit
scdc:
- 1.1.1:2:24
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '200'
type: monster
---

```ds-statblock
name: Rival Conduit
level: 8
roles:
  - Elite Support
ancestry:
  - Humanoid
  - Rival
ev: "40"
stamina: "200"
speed: 5
size: 1M
stability: 1
free_strike: 8
might: 3
agility: 0
reason: 1
intuition: 4
presence: 2
traits:
  - name: Unwavering Defender
    effects:
      - effect: Damage dealt to any ally adjacent to the conduit is halved.
  - name: Rivalry
    effects:
      - effect: At the start of an encounter, the conduit chooses one creature within
          their line of effect. Both the conduit and the creature can add a d3
          roll to power rolls they make against each other.
abilities:
  - name: Celestial Furor
    icon: ⚔️
    cost: Signature Ability
    keywords:
      - Magic
      - Melee
      - Ranged
      - Strike
    type: Main action
    distance: Melee 1 or ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        t1: 12 holy damage; vertical slide 2
        t2: 17 holy damage; vertical slide 3
        t3: 21 holy damage; vertical slide 4
      - effect: The conduit or one ally within distance regains Stamina equal to half
          the damage dealt.
        name: Effect
  - name: Imbue with Power
    icon: 🏹
    cost: 3 Malice
    keywords:
      - Magic
      - Ranged
    type: Maneuver
    distance: Ranged 10
    target: Self and five allie
    effects:
      - effect: Each target has a double edge on their next strike.
        name: Effect
```