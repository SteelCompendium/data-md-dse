---
agility: 4
ancestry:
- Human
- Humanoid
ev: '156'
file_basename: Ajax the Invincible
file_dpath: Monsters/Ajax the Invincible/Statblocks
free_strike: 11
intuition: 5
item_id: ajax-the-invincible
item_index: '138'
item_name: Ajax the Invincible
level: 11
might: 5
presence: 4
reason: 5
roles:
- Solo
scc:
- mcdm.monsters.v1:monster:ajax-the-invincible
scdc:
- 1.1.1:2:138
size: 1L
source: mcdm.monsters.v1
speed: 7
stability: 2
stamina: '700'
type: monster
---

```ds-statblock
name: Ajax the Invincible
level: 11
roles:
  - Solo
ancestry:
  - Human
  - Humanoid
ev: "156"
stamina: "700"
speed: 7
movement: Fly, hover
size: 1L
stability: 2
free_strike: 11
might: 5
agility: 4
reason: 5
intuition: 5
presence: 4
traits:
  - name: Ajax
    effects:
      - effect: Ajax takes up to three turns each round. He can't take turns
          consecutively. Additionally, he can use three triggered actions in a
          round while he isn't dazed.
        name: Ajax Turns
      - effect: At the end of each of his turns, Ajax can take 20 damage to end up to
          two effects on him that can be ended by a saving throw. This damage
          can't be reduced in any way.
        name: End Effect
  - name: I'm Not Done Yet.
    effects:
      - effect: Ajax dies only when his Stamina reaches −350. While his Stamina is below
          0, Ajax is bleeding, he can choose any two options from his Tactical
          Stance trait each round, and the Director gains 2 additional Malice
          per round.
abilities:
  - name: Blade of the Gol King
    keywords:
      - Charge
      - Magic
      - Melee
      - Strike
      - Weapon
    type: Signature Ability
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 5
        t1: 16 damage; M < 4 the target loses 1d3 Recoveries
        t2: 22 damage; M < 5 the target loses 1d3 Recoveries
        t3: 26 damage; M < 6 prone and the target loses 1d3 Recoveries
      - effect: Ajax shifts up to 2 squares between striking each target.
      - effect: Ajax can strike one additional target for each Malice spent.
        cost: 1+ Malice
  - name: Decree by the Jade Hand
    keywords:
      - Area
      - Magic
      - Ranged
    type: Main Action
    distance: 3 cube within 10
    target: Each enemy and object in the area
    effects:
      - roll: Power Roll + 5
        t1: 11 holy damage; slide 2; P < 4 the target is hexed (save ends)
        t2: 17 holy damage; slide 5; P < 5 the target is hexed (save ends)
        t3: 21 holy damage; slide 8; P < 6 the target is hexed (save ends)
      - effect: A hexed target glows green, and each of their heroic abilities has its
          cost increased by 2.
      - effect: The potency increases by 1. Additionally, the ground beneath the area
          drops 3 squares and is difficult terrain. Each flying target who has M
          < 5 is knocked prone.
        cost: 3 Malice
  - name: Divine Vine
    keywords:
      - Magic
      - Ranged
      - Weapon
    type: Maneuver
    distance: Ranged 5
    target: One creature or object 1
    effects:
      - roll: Power Roll + 5
        t1: No effect.
        t2: The target is grabbed.
        t3: 11 damage; the target is grabbed.
      - effect: If the target is grabbed, Ajax can choose to keep the vine extended,
          pull the target adjacent to him, or pull himself adjacent to the
          target. The vine stays attached to a grabbed target until it takes
          damage from a strike, the target escapes the grab, or Ajax causes the
          vine to release the target (no action required).
      - effect: This ability can be replaced with the features of a different treasure
          Ajax has acquired.
        name: Special
  - name: Bead of Hell
    cost: 2 Malice
    keywords:
      - Area
      - Magic
      - Ranged
    type: Maneuver
    distance: 5 cube within 20
    target: Special
    effects:
      - effect: Ajax throws a glowing bead to a square within distance, which ignites at
          the start of Ajax's next turn and creates an area around it that lasts
          until the start of Ajax's following turn. Each enemy in the area when
          the bead ignites takes 20 fire damage, and if they have A < 5, they
          are dazed (save ends). Any enemy who starts their turn in the area
          takes 10 fire damage.
  - name: Is This What They Taught You?
    keywords:
      - Ranged
    type: Triggered action
    distance: Ranged 10
    target: The triggering creature
    trigger: A creature within distance marks Ajax.
    effects:
      - effect: The target is marked while Ajax is marked. While the target is marked
          this way, Ajax gains an edge on power rolls against them, and whenever
          the target uses a triggered action involving their mark on Ajax, he
          can make a free strike against them.
  - name: Shieldbreaker Talisman
    keywords:
      - Magic
      - Melee
    type: Triggered action
    distance: Melee 5
    target: The triggering creature
    trigger: An enemy within distance uses an ability to reduce damage.
    effects:
      - effect: Ajax makes a free strike against the target, dealing extra damage equal
          to twice the amount that was reduced. This extra damage can't be
          reduced in any way.
  - name: Who's Hesitating?
    keywords:
      - "-"
    type: Triggered action
    distance: Self
    target: Self
    trigger: A creature uses the Hesitation is Weakness ability.
    effects:
      - effect: Ajax shifts up to his speed and can make a free strike. If the target
          has R < 4, this free strike also makes them weakened until the end of
          their next turn.
  - name: Your Obsession With Me Betrays You
    keywords:
      - Magic
      - Ranged
    type: Triggered action
    distance: Ranged 10
    target: The triggering creature
    trigger: Ajax causes a creature within distance to gain ferocity or wrath.
    effects:
      - effect: If the target has I < 4, they use a signature ability against a target
          of Ajax's choice.
  - name: You Would Flounder Your Assault?
    cost: 2 Malice
    keywords:
      - Magic
    type: Triggered action
    distance: Self
    target: Self
    trigger: A creature within 10 squares regains Stamina.
    effects:
      - effect: Ajax regains the same amount of Stamina.
  - name: Phoenix Wing King
    cost: Villain Action 1
    keywords:
      - Area
      - Magic
      - Weapon
    type: "-"
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 5
        t1: 11 fire damage; A < 4 weakened (save ends)
        t2: 17 fire damage; A < 5 weakened (save ends)
        t3: 21 fire damage; A < 6 weakened (save ends)
      - effect: Ajax flies at high speed to cut through each target, then appears in an
          unoccupied space within distance.
  - name: I've Learned Their Tricks
    cost: Villain Action 2
    keywords:
      - Area
    type: "-"
    distance: 3 burst
    target: Each enemy in the area
    effects:
      - effect: Ajax uses the shadow elf eclipse's technique to reduce each target's
          surges to 0. Additionally, until the end of the round, Ajax ignores
          edges and double edges on any target's abilities, and ignores any
          nondamaging effects of any target's damage-dealing abilities.
      - effect: This villain action can be replaced with a villain action from a
          creature any target has previously encountered.
        name: Special
  - name: Awe of the Iron Crown
    cost: Villain Action 3
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 7 burst
    target: Each enemy in the area
    effects:
      - effect: Each target who has I < 5 is knocked prone and can't stand until Ajax
          deals damage to them. For each target not knocked prone, Ajax can move
          up to his speed toward that target and use Blade of the Gol King
          against them.
```