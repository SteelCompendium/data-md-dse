---
agility: 2
ancestry:
- Fey
- Humanoid
- Wode Elf
ev: '6'
file_basename: Wode Elf Sentry
file_dpath: Monsters/Elves Wode/Statblocks
free_strike: 3
intuition: 0
item_id: wode-elf-sentry
item_index: '226'
item_name: Wode Elf Sentry
level: 1
might: 0
presence: 1
reason: 0
roles:
- Platoon Support
scc:
- mcdm.monsters.v1:monster:wode-elf-sentry
scdc:
- 1.1.1:2:226
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '30'
type: monster
---

~~~ds-statblock
name: Wode Elf Sentry
level: 1
roles:
  - Platoon Support
ancestry:
  - Fey
  - Humanoid
  - Wode Elf
ev: "6"
stamina: "30"
speed: 7
size: 1M
stability: 0
free_strike: 3
might: 0
agility: 2
reason: 0
intuition: 0
presence: 1
traits:
  - name: Masking Glamor
    effects:
      - effect: Abilities targeting the sentry that would take a bane from cover or
          concealment have a double bane instead.
abilities:
  - name: Tracer Longbow
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 5 damage
        t2: 7 damage
        t3: 9 damage; the target is marked (save ends)
      - effect: Allies gain an edge on abilities against a target marked by any wode
          elf.
        name: Effect
      - effect: The sentry targets two additional creatures or objects.
        cost: 3 Malice
  - name: Death Blossom
    icon: ❇️
    cost: 2 Malice
    keywords:
      - Area
      - Weapon
    type: Maneuver
    distance: 5 burst
    target: Each marked enemy
    effects:
      - effect: Each target takes 3 damage.
        name: Effect
~~~