---
agility: 2
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '4'
file_basename: War Dog Phosphorite
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 2
intuition: 0
item_id: war-dog-phosphorite
item_index: '350'
item_name: War Dog Phosphorite
level: 2
might: 0
presence: 0
reason: 0
roles:
- Horde Hexer
scc:
- mcdm.monsters.v1:monster:war-dog-phosphorite
scdc:
- 1.1.1:2:350
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '15'
type: monster
---

```ds-statblock
name: War Dog Phosphorite
level: 2
roles:
  - Horde Hexer
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "4"
stamina: "15"
immunities:
  - Acid 2
speed: 5
size: 1M
stability: 0
free_strike: 2
might: 0
agility: 2
reason: 0
intuition: 0
presence: 0
traits:
  - name: Loyalty Collar
    effects:
      - effect: When the phosphorite is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 1d6 damage to each adjacent enemy and object.
abilities:
  - name: Caustic Detonator
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
    type: Main action
    distance: Ranged 10
    target: One creature or object
    effects:
      - name: Effect
        effect: A detonator attaches to the target. At the end of each round, roll a
          die. On an odd result, the detonator explodes, triggering the
          following power roll.
      - roll: Power Roll + 2
        t1: 4 acid damage; M < 0 bleeding (save ends)
        t2: 6 acid damage; M < 1 bleeding (save ends)
        t3: 10 acid damage; M < 2 bleeding (save ends)
      - name: Special
        effect: A creature adjacent to the target can attempt an **Agility test** as a
          maneuver to remove the detonator.
        t1: No effect
        t2: The detonator is disarmed and destroyed.
        t3: The creature can attach the detonator to another creature or object within 5
          squares of them.
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
```