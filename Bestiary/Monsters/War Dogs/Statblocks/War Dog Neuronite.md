---
agility: 1
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '3'
file_basename: War Dog Neuronite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 1
intuition: 0
item_id: war-dog-neuronite
item_index: '379'
item_name: War Dog Neuronite
level: 1
might: 0
presence: 2
reason: 0
roles:
- Horde Defender
scc:
- mcdm.monsters.v1:monster:war-dog-neuronite
scdc:
- 1.1.1:2:379
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '20'
type: monster
---

```ds-statblock
name: War Dog Neuronite
level: 1
roles:
  - Horde Defender
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "3"
stamina: "20"
immunities:
  - Psychic 2
speed: 5
movement: Fly
size: 1M
stability: 0
free_strike: 1
might: 0
agility: 1
reason: 0
intuition: 0
presence: 2
traits:
  - name: Loyalty Collar
    effects:
      - effect: When the neuronite is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 1d6 damage to each adjacent enemy and object.
abilities:
  - name: Synlirii Grafts
    icon: ❇️
    cost: Signature Ability
    keywords:
      - Area
      - Psionic
    type: Main action
    distance: 1 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        t1: 1 psychic damage; vertical slide 1
        t2: 2 psychic damage; vertical slide 2
        t3: 3 psychic damage; vertical slide 3
  - name: Posthumous Promotion
    icon: 🏹
    keywords:
      - Magic
      - Ranged
    type: Maneuver
    distance: Ranged 10
    target: One war dog
    effects:
      - effect: If the target has a loyalty collar, they are reduced to 0 Stamina.
        name: Effect
  - name: The Voice
    icon: ❇️
    cost: 1 Malice
    keywords:
      - Area
      - Psionic
    type: Maneuver
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - effect: The neuronite chooses one ally within 10 squares. Each target is either
          taunted by the ally, or the ally has damage immunity 3 whenever any
          target makes a strike against them (the neuronite's choice). Either
          effect lasts until the start of the neuronite's next turn
        name: Effect
```