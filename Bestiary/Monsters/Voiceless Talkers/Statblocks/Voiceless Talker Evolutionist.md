---
agility: 3
ancestry:
- Horror
- Voiceless Talker
ev: '32'
file_basename: Voiceless Talker Evolutionist
file_dpath: Monsters/Voiceless Talkers/Statblocks
free_strike: 7
intuition: 1
item_id: voiceless-talker-evolutionist
item_index: '339'
item_name: Voiceless Talker Evolutionist
level: 6
might: 0
presence: 2
reason: 4
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:voiceless-talker-evolutionist
scdc:
- 1.1.1:2:339
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '180'
type: monster
---

```ds-statblock
name: Voiceless Talker Evolutionist
level: 6
roles:
  - Leader
ancestry:
  - Horror
  - Voiceless Talker
ev: "32"
stamina: "180"
immunities:
  - Psychic 8
speed: 5
movement: Hover, teleport
size: 1M
stability: 2
free_strike: 7
might: 0
agility: 3
reason: 4
intuition: 1
presence: 2
traits:
  - name: End Effect
    effects:
      - effect: At the end of each of their turns, the evolutionist can take 10 damage
          to end one effect on them that can be ended by a saving throw. This
          damage can't be reduced in any way.
  - name: Witness Evolutionary Superiority
    effects:
      - effect: The evolutionist has any trait of the Director's choice from any ally
          minion in the encounter.
abilities:
  - name: Psionic Intrusion
    cost: Signature Ability
    keywords:
      - Melee
      - Psionic
      - Ranged
      - Strike
    type: Main action
    distance: Melee 1 or ranged 5
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        t1: 11 psychic damage; R < 2 slowed (save ends)
        t2: 16 psychic damage; R < 3 slowed (save ends)
        t3: 19 psychic damage; R < 4 slowed (save ends)
  - name: Carpe Quadratum
    keywords:
      - Psionic
      - Ranged
    type: Maneuver
    distance: Ranged 5
    target: One creature
    effects:
      - effect: The evolutionist teleports to swap places with the target.
        name: Effect
  - name: Adaptability
    keywords:
      - Psionic
    type: Triggered action
    distance: Self
    target: Self
    trigger: The evolutionist takes damage that has a damage type.
    effects:
      - effect: Until the start of their next turn, the evolutionist has damage immunity
          5 to the triggering damage type.
        name: Effect
  - name: Show Me Who You Are
    cost: Villain Action 1
    keywords:
      - Area
      - Psionic
    type: "-"
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - name: Effect
        effect: Each target makes an Intuition test.
        t1: The target uses a signature ability against the nearest enemy within
          distance.
        t2: The target makes a free strike against the nearest enemy within distance.
        t3: Frightened (save ends)
  - name: Release the Thralls
    cost: Villain Action 2
    keywords:
      - Psionic
      - Ranged
    type: "-"
    distance: Ranged 5
    target: Special
    effects:
      - effect: The evolutionist teleports eight minions of level 4 or lower into
          unoccupied spaces within distance. All eight minions can be of any
          monster type but must share the same name.
        name: Effect
  - name: Brainstorm
    cost: Villain Action 3
    keywords:
      - Area
      - Psionic
    type: "-"
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        t1: 7 lightning damage
        t2: 12 lightning damage
        t3: 15 lightning damage
      - effect: Until the end of the encounter, the evolutionist is surrounded by a
          psionic electrical storm that is a 5 aura. The area is difficult
          terrain for enemies, and any enemy who enters the area for the first
          time in a round or starts their turn there takes 8 lightning damage.
        name: Effect
```