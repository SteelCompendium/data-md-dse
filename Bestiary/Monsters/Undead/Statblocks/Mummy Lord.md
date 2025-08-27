---
agility: 0
ancestry:
- Mummy
- Undead
ev: '24'
file_basename: Mummy Lord
file_dpath: Monsters/Undead/Statblocks
free_strike: 6
intuition: 4
item_id: mummy-lord
item_index: '78'
item_name: Mummy Lord
level: 4
might: 4
presence: 2
reason: 2
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:mummy-lord
scdc:
- 1.1.1:2:78
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 4
stamina: '155'
type: monster
---

```ds-statblock
name: Mummy Lord
level: 4
roles:
  - Leader
ancestry:
  - Mummy
  - Undead
ev: "24"
stamina: "155"
immunities:
  - Corruption 6
  - poison 6
weaknesses:
  - Fire 5
speed: 6
size: 1M
stability: 4
free_strike: 6
might: 4
agility: 0
reason: 2
intuition: 4
presence: 2
traits:
  - name: Cursed Transference
    effects:
      - effect: At the end of each of their turns, the mummy lord can take 10 damage to
          end one effect on them that can be ended by a saving throw. This
          damage can't be reduced in any way.
      - effect: The effect that is ended is transferred to another creature within 10
          squares.
        cost: 5 Malice
abilities:
  - name: Accursed Slam
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        t1: 10 corruption damage; I < 2 bleeding (save ends)
        t2: 14 corruption damage; I < 3 bleeding (save ends)
        t3: 17 corruption damage; I < 4 bleeding (save ends)
      - effect: While the target is bleeding this way, the potency of any ability used
          against them increases by 1 for the target.
        name: Effect
  - name: Binding Curse
    icon: 🏹
    cost: 1 Malice
    keywords:
      - Magic
      - Ranged
    type: Main action
    distance: Ranged 20
    target: One creature
    effects:
      - roll: Power Roll + 4
        t1: 7 corruption damage; I < 2 frightened (save ends)
        t2: 12 corruption damage; I < 3 frightened (save ends)
        t3: 16 corruption damage; I < 4 frightened (save ends)
      - effect: While frightened this way, a target takes 4 psychic damage whenever they
          use a move action.
        name: Effect
      - effect: This ability targets one additional target for each 2 Malice spent.
        cost: 2+ Malice
  - name: Summon My Guard
    icon: ❗️
    cost: 2 Malice
    keywords:
      - Ranged
    type: Triggered action
    distance: Ranged 10
    target: Special
    trigger: The mummy lord is made winded for the first time in the encounter.
    effects:
      - effect: One mummy or four ghoul cravers appear within distance.
        name: Effect
  - name: Plague of Flies
    icon: ☠️
    cost: Villain Action 1
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        t1: 5 poison damage
        t2: 8 poison damage
        t3: 10 poison damage
      - effect: Each target takes a bane on their next strike.
        name: Effect
  - name: Land's Guardian
    icon: ☠️
    cost: Villain Action 2
    keywords:
      - "-"
    type: "-"
    distance: Self
    target: Self
    effects:
      - name: Effect
        effect: The mummy lord gains a +2 bonus to speed and can automatically burrow at
          full speed while moving. They can then use the Dig maneuver. The next
          time the mummy lord breaches the surface, each enemy within 2 squares
          of the mummy lord makes an **Agility test**.
        t1: Prone and can't stand (EoT)
        t2: Prone
        t3: No effect
  - name: Unbound Horrors
    icon: ☠️
    cost: Villain Action 3
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        t1: 5 corruption damage; I < 2 frightened (save ends)
        t2: 8 corruption damage; I < 3 frightened (save ends)
        t3: 10 corruption damage; I < 4 frightened and restrained (save ends)
```