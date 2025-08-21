---
agility: 2
ancestry:
- Humanoid
- Orc
ev: '20'
file_basename: Orc Warleader
file_dpath: Monsters/Orcs/Statblocks
free_strike: 5
intuition: 2
item_id: orc-warleader
item_index: '128'
item_name: Orc Warleader
level: 3
might: 3
presence: 2
reason: 1
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:orc-warleader
scdc:
- 1.1.1:2:128
size: 1M
source: mcdm.monsters.v1
speed: 6
stability: 2
stamina: '120'
type: monster
---

```ds-statblock
name: Orc Warleader
level: 3
roles:
  - Leader
ancestry:
  - Humanoid
  - Orc
ev: "20"
stamina: "120"
speed: 6
size: 1M
stability: 2
free_strike: 5
might: 3
agility: 2
reason: 1
intuition: 2
presence: 2
traits:
  - name: End Effect
    effects:
      - effect: At the end of each of their turns, the warleader can take 5 damage to
          end one effect on them that can be ended by a saving throw. This
          damage can't be reduced in any way.
  - name: Relentless
    effects:
      - effect: If the warleader is reduced to 0 Stamina, they can make a free strike
          before dying. If the target of the free strike is reduced to 0
          Stamina, the warleader is reduced to 1 Stamina instead.
abilities:
  - name: Go.
    cost: Signature Ability
    keywords:
      - Ranged
    type: Main action
    distance: Ranged 10
    target: One ally
    effects:
      - effect: The target moves up to their speed and can use a main action.
        name: Effect
      - effect: The warleader targets two allies.
        cost: 1 Malice
      - effect: The warleader targets one ally and a minion squad.
        cost: 3 Malice
  - name: Mace Lariat
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: Each enemy
    effects:
      - roll: Power Roll + 3
        t1: 7 damage; push 1; M < 1 dazed (save ends)
        t2: 10 damage; push 3; M < 2 dazed (save ends)
        t3: 13 damage; push 5; M < 3 dazed (save ends)
  - name: Lockdown
    cost: 3 Malice
    keywords:
      - Ranged
    type: Maneuver
    distance: Self and ranged 10
    target: Self and three allies
    effects:
      - effect: Each target moves up to their speed and can use the Grab maneuver, which
          gains an edge.
        name: Effect
  - name: Courtesy Call
    keywords:
      - Ranged
    type: Triggered action
    distance: Ranged 10
    target: One creature
    trigger: The target obtains a tier 1 outcome on one power roll.
    effects:
      - effect: The target has a double edge on their next power roll before the end of
          the encounter.
        name: Effect
  - name: Close In
    cost: Villain Action 1
    keywords:
      - \\ Area\\
    type: "-"
    distance: 10 burst
    target: Each ally in the area
    effects:
      - name: Effect
        effect: Each target moves up to their speed. Each enemy adjacent to a target
          after this move makes an Intuition test.
        t1: Frightened of the warleader (save ends)
        t2: Frightened of the warleader (EoT)
        t3: No effect
  - name: Familial Reinforcements
    cost: Villain Action 2
    keywords:
      - Ranged
    type: "-"
    distance: Ranged 10
    target: Self
    effects:
      - effect: The warleader shifts up to their speed, and four orc blitzers appear in
          unoccupied spaces within distance.
        name: Effect
  - name: I'll Do This Myself
    cost: Villain Action 3
    keywords:
      - "-"
    type: "-"
    distance: Self
    target: Self
    effects:
      - effect: Three times in succession, the warleader shifts up to their speed and
          can use Mace Lariat.
        name: Effect
```