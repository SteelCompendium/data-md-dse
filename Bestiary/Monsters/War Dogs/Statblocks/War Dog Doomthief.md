---
agility: -1
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '7'
file_basename: War Dog Doomthief
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 3
intuition: 3
item_id: war-dog-doomthief
item_index: '388'
item_name: War Dog Doomthief
level: 5
might: 3
presence: 1
reason: 0
roles:
- Horde Defender
scc:
- mcdm.monsters.v1:monster:war-dog-doomthief
scdc:
- 1.1.1:2:388
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '40'
type: monster
---

```ds-statblock
name: War Dog Doomthief
level: 5
roles:
  - Horde Defender
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "7"
stamina: "40"
speed: 5
size: 1L
stability: 2
free_strike: 3
might: 3
agility: -1
reason: 0
intuition: 3
presence: 1
traits:
  - name: Doom Magnet
    effects:
      - effect: The doomthief emits a 3 aura of warped fate that blocks line of effect
          for any enemy ability that doesn't include them as a target
  - name: Loyalty Collar
    effects:
      - effect: When the doomthief is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 2d6 damage to each adjacent enemy and object.
abilities:
  - name: Ripper Shrikegun
    icon: 🔳
    cost: Signature Ability
    keywords:
      - Area
      - Weapon
    type: Main action
    distance: 10 x 3 line within 1
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        t1: 3 damage; push 1
        t2: 5 damage; push 3
        t3: 6 damage; push 5; A < 3 slowed (save ends)
      - effect: The doomthief can't willingly move on the same turn they use this
          ability.
        name: Effect
  - name: Expanding Doom
    icon: 👤
    cost: 4 Malice
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The doomthief has damage immunity 4 and the size of the aura from their
          Doom Magnet trait increases by 3, both until the start of their next
          turn.
        name: Effect
```