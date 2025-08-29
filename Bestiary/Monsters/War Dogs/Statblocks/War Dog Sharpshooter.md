---
agility: 2
ancestry:
- Humanoid
- Soulless
- War Dog
ev: 3 for four minions
file_basename: War Dog Sharpshooter
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 2
intuition: 0
item_id: war-dog-sharpshooter
item_index: '392'
item_name: War Dog Sharpshooter
level: 1
might: 0
presence: 0
reason: 0
roles:
- Minion Artillery
scc:
- mcdm.monsters.v1:monster:war-dog-sharpshooter
scdc:
- 1.1.1:2:392
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '3'
type: monster
---

~~~ds-statblock
name: War Dog Sharpshooter
level: 1
roles:
  - Minion Artillery
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: 3 for four minions
stamina: "3"
speed: 7
size: 1M
stability: 0
free_strike: 2
with_captain: +5 bonus to ranged distance
might: 0
agility: 2
reason: 0
intuition: 0
presence: 0
traits:
  - name: Loyalty Collar
    effects:
      - effect: When the sharpshooter is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 1d3 damage to each adjacent enemy and object.
abilities:
  - name: Bolt Launcher
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 5
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 2
        t1: 2 damage
        t2: 4 damage
        t3: 5 damage
      - effect: This ability ignores cover and concealment.
        name: Effect
~~~