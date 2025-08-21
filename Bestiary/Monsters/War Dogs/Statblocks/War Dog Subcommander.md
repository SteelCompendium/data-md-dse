---
agility: 0
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '4'
file_basename: War Dog Subcommander
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 2
intuition: 0
item_id: war-dog-subcommander
item_index: '368'
item_name: War Dog Subcommander
level: 2
might: 2
presence: 1
reason: 0
roles:
- Horde Support
scc:
- mcdm.monsters.v1:monster:war-dog-subcommander
scdc:
- 1.1.1:2:368
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '20'
type: monster
---

```ds-statblock
name: War Dog Subcommander
level: 2
roles:
  - Horde Support
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "4"
stamina: "20"
speed: 5
size: 1M
stability: 0
free_strike: 2
might: 2
agility: 0
reason: 0
intuition: 0
presence: 1
traits:
  - name: The Iron Saint Does Not Recognize Retreat
    effects:
      - effect: Each ally within 5 squares of the subcommander gains a +3 bonus to
          stability.
  - name: Loyalty Collar
    effects:
      - effect: When the subcommander is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 1d6 damage to each adjacent enemy and object.
abilities:
  - name: Command Saber
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 4 damage
        t2: 5 damage
        t3: 7 damage
      - effect: One ally within 5 squares of the subcommander can make a free strike
          against the target.
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
```