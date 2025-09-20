---
agility: 2
ancestry:
- Elemental
ev: '20'
file_basename: Essence of Storms
file_dpath: Monsters/Elementals/Statblocks
free_strike: 5
intuition: 0
item_id: essence-of-storms
item_index: '325'
item_name: Essence of Storms
level: 3
might: 1
presence: 2
reason: -1
roles:
- Elite Harrier
scc:
- mcdm.monsters.v1:monster:essence-of-storms
scdc:
- 1.1.1:2:325
size: 1S
source: mcdm.monsters.v1
speed: 8
stability: 0
stamina: '100'
type: monster
---

~~~ds-statblock
type: statblock
name: Essence of Storms
level: 3
roles:
  - Elite Harrier
ancestry:
  - Elemental
ev: "20"
stamina: "100"
immunities:
  - Lightning 5
speed: 8
movement: Fly
size: 1S
stability: 0
free_strike: 5
might: 1
agility: 2
reason: -1
intuition: 0
presence: 2
features:
  - type: feature
    feature_type: ability
    name: Bluster
    icon: ❇️
    ability_type: Signature Ability
    keywords:
      - Area
      - Magic
    usage: Main action
    distance: 1 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        tier1: 5 damage
        tier2: 5 damage, 4 lightning damage; push 1
        tier3: 5 damage, 7 lightning damage; push 3
      - name: Effect
        effect: The essence shifts up to 3 squares before or after using this ability.
  - type: feature
    feature_type: ability
    name: Convocation of Squalls
    icon: 🏹
    keywords:
      - Magic
      - Ranged
    usage: Maneuver
    distance: Ranged 5
    target: Self or one elemental
    effects:
      - name: Effect
        effect: Until the start of the essence's next turn, the target has lightning
          immunity 5.
      - cost: 3 Malice
        effect: Until the end of the encounter, a vortex surrounds the target in a 3
          aura. The area is difficult terrain for enemies. Additionally, at the
          end of each of the target's turns, they can push one creature in the
          area up to 5 squares.
  - type: feature
    feature_type: ability
    name: Thunderclap
    icon: ❗️
    cost: 1 Malice
    keywords:
      - Magic
      - Ranged
    usage: Triggered action
    distance: Ranged 5
    target: The triggering creature
    trigger: A creature within distance deals damage to the essence.
    effects:
      - name: Effect
        effect: The target takes 5 lightning damage.
  - type: feature
    feature_type: trait
    name: Fickle and Free
    icon: ⭐️
    effects:
      - effect: The essence can't be restrained, slowed, or knocked prone, and they
          ignore difficult terrain.
~~~