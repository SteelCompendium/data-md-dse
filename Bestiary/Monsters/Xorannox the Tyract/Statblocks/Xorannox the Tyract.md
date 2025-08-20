---
agility: 2
ancestry:
- Horror
- Overmind
ev: '96'
file_basename: Xorannox the Tyract
file_dpath: Monsters/Xorannox the Tyract/Statblocks
free_strike: 7
intuition: 3
item_id: xorannox-the-tyract
item_index: '319'
item_name: Xorannox the Tyract
level: 6
might: 4
presence: 3
reason: 4
roles:
- Solo
scc:
- mcdm.monsters.v1:monster:xorannox-the-tyract
scdc:
- 1.1.1:2:319
size: '3'
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '450'
type: monster
---

```ds-statblock
name: Xorannox the Tyract
level: 6
roles:
  - Solo
ancestry:
  - Horror
  - Overmind
ev: "96"
stamina: "450"
speed: 5
movement: Fly, hover
size: "3"
stability: 2
free_strike: 7
might: 4
agility: 2
reason: 4
intuition: 3
presence: 3
traits:
  - name: Solo Monster
    effects:
      - effect: At the end of each of his turns, Xorannox can take 10 damage to end one
          effect on him that can be ended by a saving throw. This damage can't
          be reduced in any way.
        name: End Effect
      - effect: Xorannox can take two turns each round. He can't take turns
          consecutively.
        name: Solo Turns
  - name: Eyes of the Tyract
    effects:
      - effect: Six unique eyestalks float around Xorannox, acting on his turn at his
          command until they are reduced to 0 Stamina. On each of Xorannox's
          turns, he directs one eyestalk to move and use a signature ability.
  - name: Above It All
    effects:
      - effect: Xorannox can't be made frightened or knocked prone, and he can't be
          flanked
  - name: Natural Enemies
    effects:
      - effect: If Xorannox perceives another overmind or a voiceless talker on the
          encounter map, he targets that threat one or more times on each of his
          turns.
abilities:
  - name: Toothful Thrashing
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creatures or object
    effects:
      - roll: Power Roll + 4
        t1: 12 damage; slide 2; M < 2 bleeding (EoT)
        t2: 20 damage; slide 3; M < 3 bleeding (EoT)
        t3: 23 damage; vertical slide 3; M < 4 bleeding (EoT)
  - name: Grav Spike
    keywords:
      - Area
      - Psionic
    type: Main action
    distance: 2 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        t1: Vertical push 3
        t2: Vertical push 5
        t3: Vertical push 7
      - effect: Xorannox shifts up to his speed before or after using this ability.
  - name: Optical Collusion
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: Xorannox commands all his eyestalks to move up to their speed.
  - name: Shutout
    cost: 2 Malice
    keywords:
      - Area
    type: Maneuver
    distance: 5 x 2 line within 1
    target: Special
    effects:
      - effect: Xorannox ends all ongoing supernatural effects and suppresses
          supernatural effects from treasures in the area. New supernatural
          effects can't be activated in the area until the end of Xorannox's
          next turn.
  - name: Cower!
    keywords:
      - Psionic
      - Ranged
    type: Triggered action
    distance: Ranged 10
    target: The triggering creature
    trigger: A creature within distance deals damage to Xorannox.
    effects:
      - effect: If the target has I < 3 they are frightened (save ends)
  - name: Disruption Beam
    cost: Villain Action 1
    keywords:
      - Psionic
      - Ranged
      - Strike
    type: "-"
    distance: Ranged 10
    target: Three creatures
    effects:
      - roll: Power Roll + 4
        t1: 11 psychic damage; R < 2 dazed (save ends)
        t2: 17 psychic damage; R < 3 dazed (save ends)
        t3: 20 psychic damage; R < 4 dazed (save ends)
  - name: All Eyes, All Rise
    cost: Villain Action 2
    keywords:
      - "-"
    type: "-"
    distance: Self
    target: Self
    effects:
      - effect: Xorannox recreates any destroyed eyestalks, which return in unoccupied
          spaces on the encounter map with full Stamina.
  - name: Panoptibeam
    cost: Villain Action 3
    keywords:
      - Area
    type: "-"
    distance: 2 burst
    target: Each enemy in the area
    effects:
      - effect: Xorannox directs each of his eyestalks to use a signature ability
          against any target.
```