---
agility: 3
ancestry:
- Beast
- Wyvern
ev: '24'
file_basename: Wyvern Lurker
file_dpath: Monsters/Wyverns/Statblocks
free_strike: 6
intuition: 1
item_id: wyvern-lurker
item_index: '121'
item_name: Wyvern Lurker
level: 4
might: 2
presence: 0
reason: -1
roles:
- Elite Ambusher
scc:
- mcdm.monsters.v1:monster:wyvern-lurker
scdc:
- 1.1.1:2:121
size: '2'
source: mcdm.monsters.v1
speed: 9
stability: 2
stamina: '120'
type: monster
---

```ds-statblock
name: Wyvern Lurker
level: 4
roles:
  - Elite Ambusher
ancestry:
  - Beast
  - Wyvern
ev: "24"
stamina: "120"
immunities:
  - Acid 5
speed: 9
movement: Fly
size: "2"
stability: 2
free_strike: 6
might: 2
agility: 3
reason: -1
intuition: 1
presence: 0
traits:
  - name: Ruthless Rage
    effects:
      - effect: While within 10 squares of another wyvern, the lurker deals an extra 3
          damage with strikes.
  - name: Tenacious Hunter
    effects:
      - effect: Any creature affected by a condition imposed by a wyvern can't be hidden
          from the lurker.
abilities:
  - name: Agonizing Stinger
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Magic
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        t1: 9 damage
        t2: 14 damage; M < 2 bleeding (save ends)
        t3: 17 damage; M < 3 bleeding (save ends)
      - effect: One target hidden from the lurker takes an extra 6 acid damage.
        cost: 1 Malice
  - name: Acidic Anguish
    icon: 🗡
    cost: 3 Malice
    keywords:
      - Magic
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: One creature or object
    effects:
      - roll: Power Roll + 3
        t1: 10 acid damage; M < 1 weakened (save ends)
        t2: 16 acid damage; M < 2 weakened (save ends)
        t3: 20 acid damage; M < 3 weakened (save ends)
      - effect: A target weakened this way takes 1d4 acid damage at the start of each of
          their turns.
        name: Effect
  - name: Swooping Torment
    icon: 👤
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The lurker flies up to their speed, then can attempt to hide. Each enemy
          the lurker moves adjacent to during this movement can choose to take 3
          sonic damage or fall prone.
        name: Effect
  - name: Retaliatory Dive
    icon: ❗️
    keywords:
      - Ranged
    type: Triggered action
    distance: Ranged 5
    target: The triggering creature
    trigger: A creature within distance deals damage to the lurker with a ranged
      ability.
    effects:
      - effect: The lurker flies adjacent to the target and can make a free strike
          against them.
        name: Effect
```