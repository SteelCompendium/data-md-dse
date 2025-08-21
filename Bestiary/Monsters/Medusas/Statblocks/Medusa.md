---
agility: 4
ancestry:
- Accursed
- Humanoid
- Medusa
ev: '84'
file_basename: Medusa
file_dpath: Monsters/Medusas/Statblocks
free_strike: 8
intuition: 0
item_id: medusa
item_index: '246'
item_name: Medusa
level: 5
might: 2
presence: 0
reason: 0
roles:
- Solo
scc:
- mcdm.monsters.v1:monster:medusa
scdc:
- 1.1.1:2:246
size: 1M
source: mcdm.monsters.v1
speed: 1
stability: 5
stamina: '0420'
type: monster
---

```ds-statblock
name: Medusa
level: 5
roles:
  - Solo
ancestry:
  - Accursed
  - Humanoid
  - Medusa
ev: "84"
stamina: "0420"
speed: 1
size: 1M
stability: 5
free_strike: 8
might: 2
agility: 4
reason: 0
intuition: 0
presence: 0
traits:
  - name: Solo Monster
    effects:
      - effect: At the end of each of their turns, the medusa can take 10 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
        name: End Effect
      - effect: The medusa can take two turns each round. They can't take turns
          consecutively.
        name: Solo Turns
  - name: Cunning Edge
    effects:
      - effect: The medusa gains an edge on power rolls against any creature who is
          restrained or slowed by Petrify.
  - name: Many Peering Eyes
    effects:
      - effect: The medusa can't be flanked
abilities:
  - name: Snake Bites
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
        t1: 11 damage; M < 2 slowed (save ends)
        t2: 16 damage; M < 3 slowed (save ends)
        t3: 19 damage; M < 4 slowed (save ends)
  - name: Damning Gaze
    cost: Signature Ability
    keywords:
      - Magic
      - Ranged
      - Strike
    type: Main action
    distance: Ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        t1: 11 damage; push 3
        t2: 16 damage; push 5
        t3: 19 damage; push 7
      - effect: The medusa targets two additional creatures or objects.
        cost: 3 Malice
  - name: Petrify
    cost: 5 Malice
    keywords:
      - Area
      - Magic
    type: Main action
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        t1: M < 2 restrained (save ends)
        t2: M < 3 restrained (save ends)
        t3: Slowed (save ends); or if M < 4 restrained (save ends)
      - effect: A target with cover reduces the potency by 1, while a slowed target
          increases the potency by 1. A target restrained this way magi- cally
          begins to turn to stone, and a target who ends two consecutive turns
          restrained this way is petrified
        name: Effect
  - name: Nimble Escape
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: The medusa shifts up to 3 squares and can attempt to hide even if
          observed.
        name: Effect
  - name: Venomous Spit
    cost: 2 Malice
    keywords:
      - Melee
    type: Triggered action
    distance: Melee 1
    target: The triggering creature
    trigger: A creature within distance deals damage to the medusa.
    effects:
      - roll: Power Roll + 4
        t1: 13 acid damage
        t2: 18 acid damage
        t3: 22 acid damage
  - name: Mass Petrify
    cost: Villain Action 1
    keywords:
      - Magic
      - Ranged
    type: "-"
    distance: Ranged 50
    target: Each enemy
    effects:
      - effect: The medusa can use Petrify against each target without spending Malice.
          A target who doesn't have cover increases the potency by 1.
        name: Effect
  - name: Serpent Wings
    cost: Villain Action 2
    keywords:
      - "-"
    type: "-"
    distance: Self
    target: Self
    effects:
      - effect: The medusa temporarily manifests wings and flies up to their speed
          without provoking opportunity attacks. During or after this movement,
          they can use Snake Bites and Damning Gaze once each.
        name: Effect
  - name: Stone Puppets
    cost: Villain Action 3
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 10 burst
    target: Special
    effects:
      - cost: ≤11
        effect: 8 acid damage; P < 3 weakened (save ends)
        t2: 13 acid damage; P < 4 weakened (save ends)
        t3: 17 acid damage; P < 5 weakened (save ends)
      - effect: As a free triggered action, each stone statue and creature restrained or
          slowed by Petrify within distance moves up to their speed and uses a
          signature ability that gains an edge, targeting an enemy of the
          medusa's choice. A stone statue without its own statistics has speed 5
          and uses the medusa's free strike.
        name: Effect
```