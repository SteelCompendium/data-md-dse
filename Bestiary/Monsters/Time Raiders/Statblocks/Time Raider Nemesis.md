---
agility: 2
ancestry:
- Humanoid
- Time Raider
ev: '10'
file_basename: Time Raider Nemesis
file_dpath: Monsters/Time Raiders/Statblocks
free_strike: 5
intuition: 1
item_id: time-raider-nemesis
item_index: '142'
item_name: Time Raider Nemesis
level: 3
might: 1
presence: 0
reason: 2
roles:
- Platoon Harrier
scc:
- mcdm.monsters.v1:monster:time-raider-nemesis
scdc:
- 1.1.1:2:142
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 0
stamina: '50'
type: monster
---

```ds-statblock
name: Time Raider Nemesis
level: 3
roles:
  - Platoon Harrier
ancestry:
  - Humanoid
  - Time Raider
ev: "10"
stamina: "50"
immunities:
  - Psychic 3
speed: 7
movement: Fly
size: 1M
stability: 0
free_strike: 5
might: 1
agility: 2
reason: 2
intuition: 1
presence: 0
traits:
  - name: Foresight
    effects:
      - effect: The nemesis doesn't take a bane on strikes against creatures with
          concealment.
abilities:
  - name: Golden Scythe
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Psionic
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 10
    target: One creature or object
    effects:
      - roll: Power Roll + 2
        t1: 7 damage; pull 1
        t2: 10 damage; pull 2
        t3: 13 damage; pull 3; A < 2 restrained (save ends)
      - effect: This ability can target creatures on parallel planes of existence and
          pull them onto the nemesis's plane.
        name: Effect
  - name: Kinetic Crush
    icon: 🏹
    cost: 2 Malice
    keywords:
      - Psionic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 10
    target: One creature
    effects:
      - roll: Power Roll + 2
        t1: 7 psychic damage; M < 0 slowed (save ends)
        t2: 10 psychic damage; M < 1 slowed (save ends)
        t3: 13 psychic damage; M < 2 slowed (save ends)
      - effect: Any creature slowed this way takes 2 damage for each square they move or
          are force moved until that condition ends.
        name: Effect
```