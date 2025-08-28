---
agility: 2
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '36'
file_basename: War Dog Breaker
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 7
intuition: 1
item_id: war-dog-breaker
item_index: '374'
item_name: War Dog Breaker
level: 7
might: 4
presence: 3
reason: 1
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:war-dog-breaker
scdc:
- 1.1.1:2:374
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 4
stamina: '200'
type: monster
---

~~~ds-statblock
name: War Dog Breaker
level: 7
roles:
  - Elite Brute
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "36"
stamina: "200"
speed: 5
size: "2"
stability: 4
free_strike: 7
might: 4
agility: 2
reason: 1
intuition: 1
presence: 3
traits:
  - name: Breaking Point
    effects:
      - effect: When the breaker would be reduced to 0 Stamina, they delay that effect
          as they end any conditions affecting them and immediately take a turn,
          regardless of whether they have already taken a turn this round. The
          breaker's abilities deal an extra 5 damage during this turn, at the
          end of which they are reduced to 0 Stamina.
  - name: Loyalty Collar
    effects:
      - effect: When the breaker is reduced to 0 Stamina, their loyalty collar explodes,
          dealing 3d6 damage to each adjacent enemy and object.
abilities:
  - name: Pile Bunker Gauntlet
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        t1: 12 damage; push 4; prone
        t2: 17 damage; slide 4; prone or M < 3 dazed (save ends)
        t3: 21 damage; slide 4; prone; M < 4 dazed (save ends)
  - name: Surging Power
    icon: 👤
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: Until the start of their next turn, the breaker has a double edge on
          abilities and is automatically affected by all potency effect
        name: Effect
~~~