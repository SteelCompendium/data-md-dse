---
agility: 4
ancestry:
- Abyssal
- Demon
- Soulraker
ev: '9'
file_basename: Soulraker Praetorian
file_dpath: Monsters/Demons/Statblocks
free_strike: 3
intuition: 2
item_id: soulraker-praetorian
item_index: '263'
item_name: Soulraker Praetorian
level: 7
might: 2
presence: 0
reason: 0
roles:
- Horde Harrier
scc:
- mcdm.monsters.v1:monster:soulraker-praetorian
scdc:
- 1.1.1:2:263
size: 1L
source: mcdm.monsters.v1
speed: 8
stability: 0
stamina: '45'
type: monster
---

```ds-statblock
name: Soulraker Praetorian
level: 7
roles:
  - Horde Harrier
ancestry:
  - Abyssal
  - Demon
  - Soulraker
ev: "9"
stamina: "45"
weaknesses:
  - Holy 5
speed: 8
size: 1L
stability: 0
free_strike: 3
might: 2
agility: 4
reason: 0
intuition: 2
presence: 0
traits:
  - name: Lethe
    effects:
      - effect: While the praetorian is winded, they gain an edge on strikes, and any
          strike made against them gains an edge.
  - name: Praetorian Buzzing
    effects:
      - effect: Any creature who starts their turn with two or more praetorians adjacent
          to them takes 6 sonic damage.
abilities:
  - name: Barbed Stinger
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: One creature
    effects:
      - roll: Power Roll + 4
        t1: 7 poison damage; push 2
        t2: 10 poison damage; push 2
        t3: 11 poison damage; push 4; A < 4 grabbed
      - effect: The praetorian can shift into each square the target leaves.
        name: Effect
  - name: Stinging Departure
    cost: 2 Malice
    keywords:
      - "-"
    type: Triggered action
    distance: Self
    target: The triggering creature
    trigger: A creature ends the praetorian's grab.
    effects:
      - effect: The praetorian makes a free strike against the target, breaks off part
          of their stinger in the target, and shifts up to half their speed. The
          target is bleeding until they remove the stinger fragment as a free
          maneuver, taking 6 damage in the process.
        name: Effect
```