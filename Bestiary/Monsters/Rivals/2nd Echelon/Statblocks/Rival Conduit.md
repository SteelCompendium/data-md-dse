---
agility: 0
ancestry:
- Humanoid
- Rival
ev: '28'
file_basename: Rival Conduit
file_dpath: Monsters/Rivals/2nd Echelon/Statblocks
free_strike: 6
intuition: 3
item_id: rival-conduit
item_index: '17'
item_name: Rival Conduit
level: 5
might: 2
presence: 1
reason: 0
roles:
- Elite Support
scc:
- mcdm.monsters.v1:monster:rival-conduit
scdc:
- 1.1.1:2:17
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '140'
type: monster
---

~~~ds-statblock
name: Rival Conduit
level: 5
roles:
  - Elite Support
ancestry:
  - Humanoid
  - Rival
ev: "28"
stamina: "140"
speed: 5
size: 1M
stability: 1
free_strike: 6
might: 2
agility: 0
reason: 0
intuition: 3
presence: 1
traits:
  - name: Stalwart Guardian
    effects:
      - effect: Strikes made against allies adjacent to the conduit take a bane.
  - name: Rivalry
    effects:
      - effect: At the start of an encounter, the conduit chooses one creature within
          their line of effect. Both the conduit and the creature can add a d3
          roll to power rolls they make against each other.
abilities:
  - name: Raging Tempest
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
      - roll: Power Roll + 3
        t1: 9 holy damage; vertical slide 1
        t2: 14 holy damage; vertical slide 2
        t3: 17 holy damage; vertical slide 3
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
~~~