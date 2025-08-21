---
agility: 2
ancestry:
- Abyssal
- Demon
ev: '20'
file_basename: Chorogaunt
file_dpath: Monsters/Demons/Statblocks
free_strike: 5
intuition: 2
item_id: chorogaunt
item_index: '258'
item_name: Chorogaunt
level: 3
might: 2
presence: 3
reason: 2
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:chorogaunt
scdc:
- 1.1.1:2:258
size: 1L
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '120'
type: monster
---

```ds-statblock
name: Chorogaunt
level: 3
roles:
  - Leader
ancestry:
  - Abyssal
  - Demon
ev: "20"
stamina: "120"
weaknesses:
  - Holy 5
speed: 5
size: 1L
stability: 2
free_strike: 5
might: 2
agility: 2
reason: 2
intuition: 2
presence: 3
traits:
  - name: End Effect
    effects:
      - effect: At the end of each of their turns, the chorogaunt can take 5 damage to
          end one effect on them that can be ended by a saving throw. This
          damage can't be reduced in any way.
  - name: Lethe
    effects:
      - effect: While the chorogaunt is winded, they gain an edge on strikes, and any
          strike made against them gains an edge.
  - name: Soulsight
    effects:
      - effect: Any creature within 2 squares of the chorogaunt can't be hidden from
          them.
abilities:
  - name: Agonizing Harmony
    cost: Signature Ability
    keywords:
      - Area
      - Weapon
    type: Main action
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        t1: 4 psychic damage; I < 1 slowed (save ends)
        t2: 7 psychic damage; I < 2 slowed (save ends)
        t3: 10 psychic damage; I < 3 slowed (save ends)
      - effect: One ally within 10 squares of the chorogaunt shifts up to their speed.
        name: Effect
  - name: Chaotic Entrancing Harmony
    keywords:
      - Area
    type: Maneuver
    distance: 10 burst
    target: Each enemy in the area
    effects:
      - effect: The chorogaunt slides each target up to 3 squares, ignoring stability.
        name: Effect
  - name: I Thrive on Pain
    cost: 3 Malice
    keywords:
      - Magic
    type: Triggered action
    distance: Self
    target: Self
    trigger: The chorogaunt is targeted by a strike.
    effects:
      - effect: Any damage from the strike is halved, and the chorogaunt's abilities
          deal an extra 3 damage until the end of their next turn.
        name: Effect
  - name: Frightening Tones
    cost: Villain Action 1
    keywords:
      - Ranged
    type: "-"
    distance: Ranged 10
    target: Three enemies
    effects:
      - effect: Each target must choose between taking 5 psychic damage, or being
          frightened (save ends).
        name: Effect
  - name: Bully the Weak
    cost: Villain Action 2
    keywords:
      - Magic
      - Ranged
    type: "-"
    distance: Ranged 10
    target: One ally
    effects:
      - effect: The chorogaunt kills the target, and each other ally in the encounter
          deals an extra 3 damage with strikes until the end of the round. The
          Director gains Malice equal to the number of heroes in the encounter.
        name: Effect
  - name: Running Cacophony
    cost: Villain Action 3
    keywords:
      - Magic
    type: "-"
    distance: Self
    target: Self
    effects:
      - effect: The chorogaunt shifts up to their speed, uses Agonizing Harmony, shifts
          up to their speed, and then uses Agonizing Harmony again.
        name: Effect
```