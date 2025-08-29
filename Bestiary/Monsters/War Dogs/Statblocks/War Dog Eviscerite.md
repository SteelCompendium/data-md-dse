---
agility: 2
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '3'
file_basename: War Dog Eviscerite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 1
intuition: 0
item_id: war-dog-eviscerite
item_index: '354'
item_name: War Dog Eviscerite
level: 1
might: 1
presence: 0
reason: 0
roles:
- Horde Harrier
scc:
- mcdm.monsters.v1:monster:war-dog-eviscerite
scdc:
- 1.1.1:2:354
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '15'
type: monster
---

~~~ds-statblock
name: War Dog Eviscerite
level: 1
roles:
  - Horde Harrier
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "3"
stamina: "15"
speed: 7
size: 1M
stability: 0
free_strike: 1
might: 1
agility: 2
reason: 0
intuition: 0
presence: 0
traits:
  - name: Loyalty Collar
    effects:
      - effect: When the eviscerite is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 1d6 damage to each adjacent enemy and object.
abilities:
  - name: Chainsaw Whip
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 3
    target: One creature and object
    effects:
      - roll: Power Roll + 2
        t1: 3 damage
        t2: 4 damage; pull 1
        t3: 5 damage; pull 2
      - effect: The eviscerite can automatically grab a target pulled adjacent to them
          this way.
        name: Effect
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
~~~