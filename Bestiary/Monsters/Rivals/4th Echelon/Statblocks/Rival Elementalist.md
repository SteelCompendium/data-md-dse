---
agility: 3
ancestry:
- Humanoid
- Rival
ev: '48'
file_basename: Rival Elementalist
file_dpath: Monsters/Rivals/4th Echelon/Statblocks
free_strike: 10
intuition: 4
item_id: rival-elementalist
item_index: '30'
item_name: Rival Elementalist
level: 10
might: 1
presence: 1
reason: 5
roles:
- Elite Controller
scc:
- mcdm.monsters.v1:monster:rival-elementalist
scdc:
- 1.1.1:2:30
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '220'
type: monster
---

~~~ds-statblock
name: Rival Elementalist
level: 10
roles:
  - Elite Controller
ancestry:
  - Humanoid
  - Rival
ev: "48"
stamina: "220"
speed: 5
size: 1M
stability: 1
free_strike: 10
might: 1
agility: 3
reason: 5
intuition: 4
presence: 1
traits:
  - name: Rivalry
    effects:
      - effect: At the start of an encounter, the elementalist chooses one creature
          within their line of effect. Both the elementalist and the creature
          can add a d3 roll to power rolls they make against each other.
abilities:
  - name: Viridescent Storm
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
      - roll: Power Roll + 5
        t1: 15 damage; slide 3; M < 3 5 acid damage
        t2: 20 damage; slide 4; M < 4 7 acid damage
        t3: 24 damage; slide 5; M < 5 9 acid damage
      - effect: One ally within distance ends all conditions on themself.
        name: Effect
  - name: The World Consumes
    icon: 🔳
    cost: 5 Malice
    keywords:
      - Area
      - Green
      - Magic
      - Ranged
    type: Main action
    distance: 3 cube within 10
    target: Each enemy in the area
    effects:
      - effect: The area becomes overgrown with caustic vines until the end of the
          encounter. While in the area, any enemy has acid weakness 5 and is
          slowed. Any enemy who ends their turn in the area and has M < 4 is
          restrained (save ends).
        name: Effect
  - name: Breach of Nihility
    icon: ❗️
    keywords:
      - Magic
      - Void
    type: Triggered action
    distance: Self
    target: Self
    trigger: The elementalist takes damage.
    effects:
      - effect: The elementalist can teleport up to 5 squares. Each creature adjacent to
          the space they leave or appear in takes 5 corruption damage.
        name: Effect
~~~