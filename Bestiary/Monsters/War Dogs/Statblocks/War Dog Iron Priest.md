---
agility: 1
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '10'
file_basename: War Dog Iron Priest
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 3
intuition: 4
item_id: war-dog-iron-priest
item_index: '351'
item_name: War Dog Iron Priest
level: 8
might: 2
presence: 4
reason: 1
roles:
- Horde Support
scc:
- mcdm.monsters.v1:monster:war-dog-iron-priest
scdc:
- 1.1.1:2:351
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '50'
type: monster
---

~~~ds-statblock
name: War Dog Iron Priest
level: 8
roles:
  - Horde Support
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "10"
stamina: "50"
speed: 5
size: 1M
stability: 0
free_strike: 3
might: 2
agility: 1
reason: 1
intuition: 4
presence: 4
traits:
  - name: Chosen of the Iron Saint
    effects:
      - effect: The Director gains 1 Malice whenever an ally within 3 squares of the
          iron priest obtains a tier 3 outcome on a power roll.
abilities:
  - name: Houndcannon
    icon: 🔳
    cost: Signature Ability
    keywords:
      - Area
      - Weapon
    type: Main action
    distance: 7 x 1 line within 1
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        t1: 3 damage
        t2: 6 damage; P < 3 bleeding (save ends)
        t3: 8 damage; P < 4 the target loses 1 Recovery and is bleeding (save ends)
      - effect: Any ally within 2 squares of the iron priest gains an edge on their next
          strike. If any target lost a Recovery, any affected ally has a double
          edge instead.
        name: Effect
  - name: Iron Banner
    icon: ❇️
    cost: 2+ Malice
    keywords:
      - Area
      - Magic
    type: Maneuver
    distance: 4 aura
    target: Each war dog in the area
    effects:
      - effect: >-
          For every 2 Malice spent, each target gains one of the following
          effects until the start of the iron priest's next turn

          - The target has damage immunity 2.

          - The target's strikes deal an extra 3 holy damage.

          - The target has a +3 bonus to speed.
        name: Effect
~~~