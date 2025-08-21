---
agility: 1
ancestry:
- Humanoid
- Kobold
ev: '3'
file_basename: Kobold Signifer
file_dpath: Monsters/Kobolds/Statblocks
free_strike: 1
intuition: 0
item_id: kobold-signifer
item_index: '89'
item_name: Kobold Signifer
level: 1
might: 0
presence: 2
reason: 0
roles:
- Horde Support
scc:
- mcdm.monsters.v1:monster:kobold-signifer
scdc:
- 1.1.1:2:89
size: 1S
source: mcdm.monsters.v1
speed: 5
stability: 0
stamina: '15'
type: monster
---

```ds-statblock
name: Kobold Signifer
level: 1
roles:
  - Horde Support
ancestry:
  - Humanoid
  - Kobold
ev: "3"
stamina: "15"
speed: 5
size: 1S
stability: 0
free_strike: 1
might: 0
agility: 1
reason: 0
intuition: 0
presence: 2
traits:
  - name: Shield? Shield!
    effects:
      - effect: While adjacent to an ally who also has this trait, the signifer has
          stability 1, has cover, and grants cover to allies.
  - name: Upholding High Standards
    effects:
      - effect: Any ally who starts their turn within 5 squares of the signifer gains a
          +2 bonus to speed and a +2 damage bonus to strikes until the end of
          their turn. Additionally, if the signifer is killed, any kobold minion
          can enter their space during the same encounter to retrieve the signum
          battle standard they carry (no action required) and replace their stat
          block with the signifer stat block.
abilities:
  - name: Signum
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
        t1: 3 damage
        t2: 4 damage
        t3: 5 damage
      - effect: One ally within 10 squares of the signifer can shift up to their speed
          if they end that shift adjacent to an ally
        name: Effect
      - effect: One additional ally can shift for each 2 Malice spent
        cost: 2+ Malice
  - name: Glory to the Legion
    cost: 5 Malice
    keywords:
      - Area
    type: Maneuver
    distance: 5 burst
    target: Each ally in the area
    effects:
      - effect: Each target regains 5 Stamina.
        name: Effect
```