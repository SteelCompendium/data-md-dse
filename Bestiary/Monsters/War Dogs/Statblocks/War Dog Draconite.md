---
agility: 1
ancestry:
- Humanoid
- Soulless
- War Dog
ev: 9 for four minions
file_basename: War Dog Draconite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 4
intuition: -1
item_id: war-dog-draconite
item_index: '362'
item_name: War Dog Draconite
level: 7
might: 4
presence: 2
reason: -2
roles:
- Minion Brute
scc:
- mcdm.monsters.v1:monster:war-dog-draconite
scdc:
- 1.1.1:2:362
size: '2'
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '13'
type: monster
---

```ds-statblock
name: War Dog Draconite
level: 7
roles:
  - Minion Brute
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: 9 for four minions
stamina: "13"
speed: 5
size: "2"
stability: 2
free_strike: 4
with_captain: +3 damage bonus to strikes
might: 4
agility: 1
reason: -2
intuition: -1
presence: 2
traits:
  - name: Loyalty Collar
    effects:
      - effect: When the draconite is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 2d6 damage to each adjacent enemy and object.
abilities:
  - name: Greatsword and Roar
    cost: Signature Ability
    keywords:
      - Charge
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: One creature or object per minion
    effects:
      - roll: Power Roll + 4
        t1: 4 damage
        t2: 4 damage, 3 psychic damage
        t3: 4 damage, 4 psychic damage; the target must move their speed in a straight
          line away from the draconite
      - effect: If this damage leaves the target winded, they are frightened of the
          draconite until the end of the target's next turn.
```