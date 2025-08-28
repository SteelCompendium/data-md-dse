---
agility: 0
ancestry:
- Humanoid
- Soulless
- War Dog
ev: 6 for four minions
file_basename: War Dog Sparkslinger
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 3
intuition: 0
item_id: war-dog-sparkslinger
item_index: '369'
item_name: War Dog Sparkslinger
level: 4
might: 0
presence: 2
reason: 3
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster:war-dog-sparkslinger
scdc:
- 1.1.1:2:369
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '7'
type: monster
---

~~~ds-statblock
name: War Dog Sparkslinger
level: 4
roles:
  - Minion Artillery
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: 6 for four minions
stamina: "7"
immunities:
  - Lightning 4
speed: 5
size: 1M
stability: 0
free_strike: 3
with_captain: Lightning spread increases by 1 square
might: 0
agility: 0
reason: 3
intuition: 0
presence: 2
traits:
  - name: Loyalty Collar
    effects:
      - effect: When the sparkslinger is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 1d6 damage to each adjacent enemy and object.
abilities:
  - name: Galvanic Arc
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 7
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 3
        t1: 3 lightning damage
        t2: 5 lightning damage; the lightning spreads 1 square
        t3: 7 lightning damage; the lightning spreads 2 squares
      - effect: The lightning's spread is the distance it arcs from a target to nearby
          enemies. Each enemy within that distance takes 2 lightning damage.
        name: Effect
~~~