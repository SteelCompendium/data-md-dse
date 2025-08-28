---
agility: 0
ancestry:
- Soulless
- War Dog
ev: '10'
file_basename: War Dog Prismite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 3
intuition: 2
item_id: war-dog-prismite
item_index: '365'
item_name: War Dog Prismite
level: 8
might: 4
presence: 3
reason: 4
roles:
- Horde Defender
scc:
- mcdm.monsters.v1:monster:war-dog-prismite
scdc:
- 1.1.1:2:365
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '82'
type: monster
---

~~~ds-statblock
name: War Dog Prismite
level: 8
roles:
  - Horde Defender
ancestry:
  - Soulless
  - War Dog
ev: "10"
stamina: "82"
speed: 5
movement: Fly, hover
size: "2"
stability: 2
free_strike: 3
might: 4
agility: 0
reason: 4
intuition: 2
presence: 3
traits:
  - name: Prismacore Detonation
    effects:
      - effect: When the prismite is reduced to 0 Stamina, they explode, dealing 3d6
          psychic damage to each enemy within 2 squares of them.
abilities:
  - name: Grasping Tonguetacles
    icon: ❇️
    cost: Signature Ability
    keywords:
      - Area
      - Psionic
      - Weapon
    type: Main action
    distance: 2 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        t1: 3 psychic damage
        t2: 6 psychic damage; R < 3 grabbed, pull 2
        t3: 8 psychic damage; R < 4 grabbed and the target takes a bane on the Escape
          Grab maneuver, pull 2
  - name: Hard Light Field
    icon: 🔳
    keywords:
      - Area
      - Psionic
      - Ranged
    type: Maneuver
    distance: 4 cube within 10
    target: Each ally in the area
    effects:
      - effect: Until the start of the prismite's next turn, each target has cover and
          gains a +2 bonus to stability.
        name: Effect
  - name: Tractor Beam
    icon: ❗️
    cost: 1 Malice
    keywords:
      - Psionic
      - Ranged
    type: Triggered action
    distance: Ranged 10
    target: The triggering enemy
    trigger: An enemy within distance uses a melee ability against an ally.
    effects:
      - effect: The target is pulled up to 5 squares toward the prismite and any damage
          from the triggering ability is halved.
        name: Effect
~~~