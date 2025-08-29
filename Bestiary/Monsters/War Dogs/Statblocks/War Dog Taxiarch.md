---
agility: 3
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '44'
file_basename: War Dog Taxiarch
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 9
intuition: 4
item_id: war-dog-taxiarch
item_index: '374'
item_name: War Dog Taxiarch
level: 9
might: 1
presence: 3
reason: 5
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:war-dog-taxiarch
scdc:
- 1.1.1:2:374
size: 1M
source: mcdm.monsters.v1
speed: 7
stability: 1
stamina: '240'
type: monster
---

~~~ds-statblock
name: War Dog Taxiarch
level: 9
roles:
  - Leader
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "44"
stamina: "240"
speed: 7
movement: Teleport
size: 1M
stability: 1
free_strike: 9
might: 1
agility: 3
reason: 5
intuition: 4
presence: 3
traits:
  - name: End Effect
    effects:
      - effect: At the end of each of their turns, the taxiarch can take 15 damage to
          end one effect on them that can be ended by a saving throw. This
          damage can't be reduced in any way.
abilities:
  - name: Stunning Surge
    icon: 🏹
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 5
        t1: 14 lightning damage; the lightning spreads 1 square; I < 3 dazed (save ends)
        t2: 19 lightning damage; the lightning spreads 2 squares; I < 4 dazed (save
          ends)
        t3: 23 lightning damage; the lightning spreads 3 squares; I < 5 dazed (save
          ends)
      - effect: The spread is the distance the charge arcs from a target to nearby
          enemies. Each enemy within spread takes 5 lightning damage.
        name: Effect
      - effect: The lighting spread increases by 2 squares. Additionally, any creature
          who takes lightning damage from this ability and who has M < 4 is
          slowed until the end of their next turn.
        cost: 2 Malice
  - name: Overcharge
    icon: 🔳
    cost: 2 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    type: Maneuver
    distance: 4 cube within 10
    target: Each war dog in the area
    effects:
      - effect: Each target shifts up to their speed and can make a free strike that
          deals an extra 5 lightning damage.
        name: Effect
  - name: Thunderstruck
    icon: ❗️
    keywords:
      - Magic
      - Melee
    type: Triggered action
    distance: Melee 1
    target: The triggering enemy
    trigger: An enemy within distance deals damage to the taxiarch.
    effects:
      - effect: After the ability is resolved, the target is teleported up to 5 squares
          and is thunderstruck (save ends). A thunderstruck creature has
          lightning weakness 5, and the taxiarch gains an edge on power rolls
          against them.
        name: Effect
  - name: Magnetic Trickery
    icon: ☠️
    cost: Villain Action 1
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 10 burst
    target: Each enemy in the area
    effects:
      - effect: Slide 5, and if the the target has M < 4, they fall prone.
        name: Effect
  - name: Conductor of Combat
    icon: ☠️
    cost: Villain Action 2
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 5 burst
    target: Each war dog in the area
    effects:
      - effect: Each target shifts up to their speed, then can make a free strike or use
          a maneuver.
        name: Effect
  - name: Unlimited Power!
    icon: ☠️
    cost: Villain Action 3
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 3 burst
    target: Each creature in the area
    effects:
      - name: Effect
        effect: Each target makes an Agility test.
        t1: 18 lightning damage; the target is thunderstruck (save ends)
        t2: 14 lightning damage; the target is thunderstruck (EoT)
        t3: 9 lightning damage
      - effect: See Thunderstruck. Additionally, until the end of the encounter, any
          enemy who moves within 3 squares of the taxiarch for the first time in
          a round or starts their turn there takes 3 lightning damage.
~~~