---
agility: 2
ancestry:
- Humanoid
- Rival
ev: '28'
file_basename: Rival Elementalist
file_dpath: Monsters/Rivals/2nd Echelon/Statblocks
free_strike: 6
intuition: 2
item_id: rival-elementalist
item_index: '16'
item_name: Rival Elementalist
level: 5
might: 0
presence: 0
reason: 3
roles:
- Elite Controller
scc:
- mcdm.monsters.v1:monster:rival-elementalist
scdc:
- 1.1.1:2:16
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '120'
type: monster
---

```ds-statblock
name: Rival Elementalist
level: 5
roles:
  - Elite Controller
ancestry:
  - Humanoid
  - Rival
ev: "28"
stamina: "120"
speed: 5
size: 1M
stability: 1
free_strike: 6
might: 0
agility: 2
reason: 3
intuition: 2
presence: 0
traits:
  - name: Rivalry
    effects:
      - effect: At the start of an encounter, the elementalist chooses one creature
          within their line of effect. Both the elementalist and the creature
          can add a d3 roll to power rolls they make against each other.
abilities:
  - name: The Thriving Wilds
    icon: 🏹
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
      - roll: Power Roll + 3
        t1: 9 damage; slide 1; M < 1 3 acid damage
        t2: 14 damage; slide 2; M < 2 5 acid damage
        t3: 17 damage; slide 3; M < 3 7 acid damage
  - name: The Depths Hunger
    icon: 🔳
    cost: 4 Malice
    keywords:
      - Area
      - Green
      - Magic
      - Ranged
    type: Main action
    distance: 4 cube within 10
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        t1: 5 damage
        t2: 9 damage; restrained (EoT)
        t3: 11 damage; restrained (save ends)
      - effect: The area is difficult terrain for enemies until the end of the
          encounter. Any enemy in the area has acid weakness 3.
        name: Effect
  - name: Fissures of Darkness
    icon: ❗️
    keywords:
      - Magic
      - Void
    type: Triggered action
    distance: Self
    target: Self
    trigger: The elementalist takes damage.
    effects:
      - effect: The elementalist can teleport up to 3 squares. Each creature adjacent to
          the space they leave takes 3 corruption damage.
        name: Effect
```