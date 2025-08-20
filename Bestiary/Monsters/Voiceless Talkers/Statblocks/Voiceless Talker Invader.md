---
agility: 1
ancestry:
- Horror
- Voiceless Talker
ev: '32'
file_basename: Voiceless Talker Invader
file_dpath: Monsters/Voiceless Talkers/Statblocks
free_strike: 7
intuition: 2
item_id: voiceless-talker-invader
item_index: '341'
item_name: Voiceless Talker Invader
level: 6
might: -1
presence: 2
reason: 3
roles:
- Elite Controller
scc:
- mcdm.monsters.v1:monster:voiceless-talker-invader
scdc:
- 1.1.1:2:341
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '140'
type: monster
---

```ds-statblock
name: Voiceless Talker Invader
level: 6
roles:
  - Elite Controller
ancestry:
  - Horror
  - Voiceless Talker
ev: "32"
stamina: "140"
immunities:
  - Psychic 6
speed: 5
movement: Hover, teleport
size: 1M
stability: 2
free_strike: 7
might: -1
agility: 1
reason: 3
intuition: 2
presence: 2
traits:
  - name: Psionic Amplifier
    effects:
      - effect: Whenever a non-minion voiceless talker within 5 squares of the invader
          uses a psionic ability, they can do so as if they were in the
          invader's space, and the ability has a double edge.
abilities:
  - name: Tentacle
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 2
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 3
        t1: 10 damage
        t2: 15 damage; M < 2 grabbed
        t3: 18 damage; M < 3 grabbed
  - name: Psionic Boom
    cost: 3 Malice
    keywords:
      - Area
      - Psionic
    type: Main action
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 3
        t1: 6 psychic damage; R < 1 push 2
        t2: 10 psychic damage; R < 2 push 3
        t3: 12 psychic damage; R < 3 push 4 and prone
      - effect: The size of the burst increases to 5.
        cost: 2 Malice
  - name: Tentacle Toss
    keywords:
      - Melee
      - Psionic
    type: Maneuver
    distance: Melee 1
    target: One creature
    effects:
      - effect: The target must be grabbed by the invader.
      - roll: Power Roll + 3
        t1: 6 damage; vertical slide 2
        t2: 10 damage; vertical slide 2
        t3: 12 damage; vertical slide 3
  - name: Brain Drain
    keywords:
      - Melee
      - Psionic
    type: Triggered action
    distance: Special
    target: The triggering creature
    trigger: A creature grabbed by the invader resists an ability's potency.
    effects:
      - effect: The potency increases by 2.
```