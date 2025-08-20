---
agility: 1
ancestry:
- Humanoid
- Kobold
ev: '3'
file_basename: Kobold Adeptus
file_dpath: Monsters/Kobolds/Statblocks
free_strike: 2
intuition: 0
item_id: kobold-adeptus
item_index: '90'
item_name: Kobold Adeptus
level: 1
might: 0
presence: 0
reason: 2
roles:
- Horde Artillery
scc:
- mcdm.monsters.v1:monster:kobold-adeptus
scdc:
- 1.1.1:2:90
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '10'
type: monster
---

```ds-statblock
name: Kobold Adeptus
level: 1
roles:
  - Horde Artillery
ancestry:
  - Humanoid
  - Kobold
ev: "3"
stamina: "10"
speed: 5
size: 1S
stability: 0
free_strike: 2
might: 0
agility: 1
reason: 2
intuition: 0
presence: 0
traits:
  - name: Shield? Shield!
    effects:
      - effect: While adjacent to an ally who also has this trait, the adeptus has
          stability 1, has cover, and grants cover to allies.
abilities:
  - name: Shocking Bolt
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 15
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 4 lightning damage
        t2: 6 lightning damage
        t3: 7 lightning damage
      - effect: While the target is adjacent to any enemy, the adeptus gains an edge on
          this ability. Each enemy adjacent to the target takes 2 lighting
          damage.
  - name: Arcane Telum
    cost: 3 Malice
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Maneuver
    distance: Ranged 15
    target: Three creatures or objects
    effects:
      - roll: Power Roll + 2
        t1: 3 damage
        t2: 5 damage
        t3: 6 damage
      - effect: This ability ignores banes, double banes, and damage immunity.
```