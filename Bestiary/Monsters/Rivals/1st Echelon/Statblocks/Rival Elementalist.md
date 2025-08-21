---
agility: 0
ancestry:
- Humanoid
- Rival
ev: '16'
file_basename: Rival Elementalist
file_dpath: Monsters/Rivals/1st Echelon/Statblocks
free_strike: 5
intuition: 1
item_id: rival-elementalist
item_index: 09
item_name: Rival Elementalist
level: 2
might: 0
presence: 0
reason: 2
roles:
- Elite Controller
scc:
- mcdm.monsters.v1:monster:rival-elementalist
scdc:
- 1.1.1:2:09
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '60'
type: monster
---

```ds-statblock
name: Rival Elementalist
level: 2
roles:
  - Elite Controller
ancestry:
  - Humanoid
  - Rival
ev: "16"
stamina: "60"
speed: 5
size: 1M
stability: 1
free_strike: 5
might: 0
agility: 0
reason: 2
intuition: 1
presence: 0
traits:
  - name: Rivalry
    effects:
      - effect: At the start of an encounter, the elementalist chooses one creature
          within their line of effect. Both the elementalist and the creature
          can add a d3 roll to power rolls they make against each other.
abilities:
  - name: The Writhing Green
    cost: Signature Ability
    keywords:
      - Green
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        t1: 7 damage; slide 1
        t2: 10 damage; slide 2
        t3: 13 damage; slide 3
  - name: The Earth Devours
    cost: 3 Malice
    keywords:
      - Area
      - Green
      - Magic
      - Ranged
    type: Main action
    distance: 3 cube within 10
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        t1: 3 damage
        t2: 5 damage; restrained (EoT)
        t3: 8 damage; restrained (save ends)
      - effect: The area is difficult terrain for enemies until the end of the
          encounter. Any enemy in the area has acid weakness 2.
        name: Effect
  - name: Jaws of the Void
    keywords:
      - Magic
      - Void
    type: Triggered action
    distance: Self
    target: Self
    trigger: The elementalist takes damage.
    effects:
      - effect: The elementalist can teleport up to 2 squares. Each creature adjacent to
          the space they leave takes 2 corruption damage.
        name: Effect
```