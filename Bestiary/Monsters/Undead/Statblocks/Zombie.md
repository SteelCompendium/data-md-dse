---
agility: 1
ancestry:
- Undead
- Soulless
ev: '3'
file_basename: Zombie
file_dpath: Monsters/Undead/Statblocks
free_strike: 2
intuition: -2
item_id: zombie
item_index: '79'
item_name: Zombie
level: 1
might: 2
presence: 1
reason: -5
roles:
- Horde Brute
scc:
- mcdm.monsters.v1:monster:zombie
scdc:
- 1.1.1:2:79
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 1
stamina: '20'
type: monster
---

```ds-statblock
name: Zombie
level: 1
roles:
  - Horde Brute
ancestry:
  - Undead
  - Soulless
ev: "3"
stamina: "20"
immunities:
  - Corruption 1
  - poison 1
speed: 5
size: 1M
stability: 1
free_strike: 2
might: 2
agility: 1
reason: -5
intuition: -2
presence: 1
traits:
  - name: Endless Knight
    effects:
      - effect: The first time the zombie is reduced to 0 Stamina by damage that isn't
          fire damage or holy damage and their body isn't destroyed, they
          instead have 10 Stamina and fall prone
abilities:
  - name: Clobber and Clutch
    icon: 🗡
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
        t2: 6 damage
        t3: 7 damage; grabbed
      - effect: "A target who starts their turn grabbed by the zombie takes 2 corruption
          damage. A creature who takes 5 or more corruption damage this way
          becomes insatiably hungry for flesh, and must complete the Find a Cure
          downtime project in Draw Steel: Heroes to end this effect"
        name: Effect
  - name: Zombie Dust
    icon: ❇️
    cost: 3 Malice
    keywords:
      - Area
    type: Maneuver
    distance: 2 burst
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: The zombie falls prone, expelling a wave of rot and dust.
      - roll: Power Roll + 2
        t1: 2 corruption damage
        t2: 3 corruption damage; M < 1 weakened (save ends)
        t3: 4 corruption damage; M < 2 dazed (save ends)
```