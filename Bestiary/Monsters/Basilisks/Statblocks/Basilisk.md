---
agility: 0
ancestry:
- Basilisk
- Beast
ev: '12'
file_basename: Basilisk
file_dpath: Monsters/Basilisks/Statblocks
free_strike: 5
intuition: -1
item_id: basilisk
item_index: '333'
item_name: Basilisk
level: 1
might: 2
presence: -1
reason: -3
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:basilisk
scdc:
- 1.1.1:2:333
size: '2'
source: mcdm.monsters.v1
speed: 8
stability: 2
stamina: '80'
type: monster
---

```ds-statblock
name: Basilisk
level: 1
roles:
  - Elite Brute
ancestry:
  - Basilisk
  - Beast
ev: "12"
stamina: "80"
immunities:
  - Poison 4
speed: 8
size: "2"
stability: 2
free_strike: 5
might: 2
agility: 0
reason: -3
intuition: -1
presence: -1
traits:
  - name: Calcifying Presence
    effects:
      - effect: The area within 3 squares of the basilisk is difficult terrain for
          enemies.
abilities:
  - name: Noxious Bite
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main Action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 2
        t1: 7 poison damage
        t2: 10 poison damage
        t3: 13 poison damage
      - effect: This ability gains an edge against targets the basilisk has previously
          dealt poison damage to.
        name: Effect
  - name: Petrifying Eye Beams
    keywords:
      - Area
      - Magic
    type: Maneuver
    distance: 5 × 2 line within 1
    target: Special
    effects:
      - name: Special
        effect: The area extends from both the basilisk's eyes, and this ability targets
          the first creature without cover on either side of the area.
      - roll: Power Roll + 2
        t1: M < 0 restrained (save ends)
        t2: M < 1 restrained (save ends)
        t3: Slowed (save ends); or if M < 2 restrained (save ends)
      - effect: If a target is already slowed, the potency increases by 1 for that
          target. A target restrained this way magically begins to turn to
          stone, and a target who ends two consecutive turns restrained this way
          is petrified. A target restrained this way or a creature adjacent to
          them can use a main action to cut encroaching stone from the target's
          body, dealing 8 damage to the target that can't be reduced in any way
          and ending this effect.
        name: Effect
  - name: Poison Fumes
    cost: 5 Malice
    keywords:
      - Area
      - Magic
    type: Main action
    distance: 3 cube within 1
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 2
        t1: 4 poison damage; M < 0 weakened (save ends)
        t2: 6 poison damage; M < 1 weakened and slowed (save ends)
        t3: 9 poison damage; M < 2 weakened and slowed (save ends)
  - name: Lash Out
    keywords:
      - Area
    type: Triggered action
    distance: 1 burst
    target: Each enemy in the area
    trigger: The basilisk takes damage from a melee ability.
    effects:
      - effect: Each target takes 5 damage. Any target who has A < 2 is also bleeding
          (save ends).
        name: Effect
```