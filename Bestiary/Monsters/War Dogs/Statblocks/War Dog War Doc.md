---
agility: 1
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '7'
file_basename: War Dog War Doc
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 3
intuition: 2
item_id: war-dog-war-doc
item_index: '386'
item_name: War Dog War Doc
level: 5
might: 0
presence: 0
reason: 3
roles:
- Horde Support
scc:
- mcdm.monsters.v1:monster:war-dog-war-doc
scdc:
- 1.1.1:2:386
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '35'
type: monster
---

```ds-statblock
name: War Dog War Doc
level: 5
roles:
  - Horde Support
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "7"
stamina: "35"
speed: 5
size: 1L
stability: 1
free_strike: 3
might: 0
agility: 1
reason: 3
intuition: 2
presence: 0
traits:
  - name: Body Bank Branch Manager
    effects:
      - effect: If the war doc uses the Reconstitute war dog Malice feature, it costs 1
          Malice less. Additionally, allies can treat the living war doc as a
          corpse when using the Reconstitute feature (see Reconstitute)
abilities:
  - name: Syringe Crossbow
    cost: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 10
    target: One creature
    effects:
      - roll: Power Roll + 3
        t1: 6 poison damage
        t2: 8 poison damage
        t3: 9 poison damage; M < 3 weakened (save ends)
      - effect: A target enemy is subject to this ability's power roll. A target ally
          instead gains 5 temporary Stamina and can make a free strike.
        name: Effect
  - name: Posthumous Promotion
    keywords:
      - Magic
      - Ranged
    type: Maneuver
    distance: Ranged 10
    target: One war dog
    effects:
      - effect: If the target has a loyalty collar, they are reduced to 0 Stamina.
        name: Effect
  - name: Sanguine Stimulants
    cost: 1 Malice
    keywords:
      - Magic
      - Ranged
    type: Triggered action
    distance: Ranged 15
    target: Special
    trigger: One ally within distance dies.
    effects:
      - effect: Each ally adjacent to the dead ally deals an extra 6 damage on their
          next strike.
        name: Effect
```