---
agility: 2
ancestry:
- Humanoid
- Soulless
- War Dog
ev: '20'
file_basename: War Dog Ground Commander
file_dpath: Monsters/War Dogs/Statblocks
free_strike: 5
intuition: 2
item_id: war-dog-ground-commander
item_index: '357'
item_name: War Dog Ground Commander
level: 3
might: 3
presence: 2
reason: 3
roles:
- Leader
scc:
- mcdm.monsters.v1:monster:war-dog-ground-commander
scdc:
- 1.1.1:2:357
size: 1M
source: mcdm.monsters.v1
speed: 5
stability: 2
stamina: '120'
type: monster
---

~~~ds-statblock
name: War Dog Ground Commander
level: 3
roles:
  - Leader
ancestry:
  - Humanoid
  - Soulless
  - War Dog
ev: "20"
stamina: "120"
speed: 5
size: 1M
stability: 2
free_strike: 5
might: 3
agility: 2
reason: 3
intuition: 2
presence: 2
traits:
  - name: End Effect
    effects:
      - effect: At the end of each of their turns, the ground commander can take 5
          damage to end one effect on them that can be ended by a saving throw.
          This damage can't be reduced in any way.
  - name: Loyalty Collar
    effects:
      - effect: When the ground commander is reduced to 0 Stamina, their loyalty collar
          explodes, dealing 2d6 damage to each adjacent enemy and object.
abilities:
  - name: Conditioning Spear
    icon: ⚔️
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
      - roll: Power Roll + 3
        t1: 8 damage; pull 1
        t2: 12 damage; pull 2
        t3: 15 damage; pull 3
      - effect: One ally within 10 squares of the ground commander can make a free
          strike.
        name: Effect
      - effect: A target who has I < 2 and who is adjacent to the ground commander after
          this ability is resolved is grabbed (save ends). This grab can't be
          escaped using the Escape Grab maneuver. The ground commander can grab
          up to two creatures at a time.
        cost: 1 Malice
  - name: Highest Posthumous Promotion
    icon: ❇️
    keywords:
      - Area
      - Magic
    type: Maneuver
    distance: 10 burst
    target: Each war dog in the area
    effects:
      - effect: Any target who has a loyalty collar is reduced to 0 Stamina.
        name: Effect
  - name: Final Orders
    icon: ❗️
    keywords:
      - Magic
      - Ranged
    type: Triggered action
    distance: Ranged 10
    target: One ally
    trigger: The target takes damage, is force moved, or is reduced to 0 Stamina.
    effects:
      - effect: Even if reduced to 0 Stamina, the target moves up to their speed and can
          make a free strike after the triggering effect is resolved The target
          then immediately dies.
        name: Effect
  - name: Combined Arms
    icon: ☠️
    cost: Villain Action 1
    keywords:
      - Area
    type: "-"
    distance: 10 burst
    target: Each ally in the area
    effects:
      - effect: Each target can make a ranged free strike, then immediately use the
          Charge main action.
        name: Effect
  - name: Make an Example of Them
    icon: ☠️
    cost: Villain Action 2
    keywords:
      - Magic
      - Ranged
    type: "-"
    distance: Ranged 10
    target: One enemy
    effects:
      - effect: Each ally within 5 squares of the target moves up to their speed and can
          make a free strike against the target. If the target has I < 2, they
          are frightened of the ground commander (save ends).
        name: Effect
  - name: Claim Them for the Body Banks
    icon: ☠️
    cost: Villain Action 3
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 10 burst
    target: Each creature in the area
    effects:
      - effect: Each target ally shifts up to 2 squares and can use the Grab maneuver.
          Until the end of the encounter, each target enemy takes a bane on the
          Escape Grab maneuver.
        name: Effect
~~~