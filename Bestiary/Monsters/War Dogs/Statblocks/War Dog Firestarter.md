---
agility: 2
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '10'
file_basename: War Dog Firestarter
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 3
intuition: 4
item_id: war-dog-firestarter
item_index: '393'
item_name: War Dog Firestarter
level: 8
might: 0
presence: 1
reason: 3
roles:
- Horde Hexer
scc:
- mcdm.monsters.v1:monster:war-dog-firestarter
scdc:
- 1.1.1:2:393
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '45'
type: monster
---

```ds-statblock
name: War Dog Firestarter
level: 8
roles:
  - Horde Hexer
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "10"
stamina: "45"
immunities:
  - Fire 8
speed: 5
size: 1M
stability: 0
free_strike: 3
might: 0
agility: 2
reason: 3
intuition: 4
presence: 1
traits:
  - name: Loyalty Collar
    effects:
      - effect: When the firestarter is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 3d6 damage to each adjacent enemy and object.
abilities:
  - name: Twin Flamebelchers
    cost: Signature Ability
    keywords:
      - Area
      - Weapon
    type: Main action
    distance: 10 x 1 line within 1
    target: Each creature and object in the area
    effects:
      - roll: Power Roll + 4
        t1: 3 fire damage; A < 2 the target is seared (save ends)
        t2: 6 fire damage; A < 3 the target is seared (save ends)
        t3: 8 fire damage; A < 4 the target is seared (save ends)
      - effect: A seared creature takes a bane on strikes and has damage weakness 5. If
          this ability obtains a tier 3 outcome against one or more creatures
          who are already seared, the firestarter can use Enflame as a free
          triggered action
        name: Effect
  - name: Enflame
    keywords:
      - Magic
      - Ranged
    type: Maneuver
    distance: Ranged 10
    target: Special
    effects:
      - name: Effect
        effect: This ability targets each enemy within 2 squares of any seared creature
          within distance.
        t1: 2 fire damage
        t2: 4 fire damage; A < 3 the target is seared (save ends)
        t3: 6 fire damage; A < 4 the target is seared (save ends)
```