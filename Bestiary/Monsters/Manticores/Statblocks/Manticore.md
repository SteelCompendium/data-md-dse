---
agility: 3
ancestry:
- Beast
- Manticore
ev: '72'
file_basename: Manticore
file_dpath: Monsters/Manticores/Statblocks
free_strike: 6
intuition: 0
item_id: manticore
item_index: '346'
item_name: Manticore
level: 4
might: 4
presence: -1
reason: 0
roles:
- Solo
scc:
- mcdm.monsters.v1:monster:manticore
scdc:
- 1.1.1:2:346
size: '2'
source: mcdm.monsters.v1
speed: 1
stability: 2
stamina: '0350'
type: monster
---

~~~ds-statblock
name: Manticore
level: 4
roles:
  - Solo
ancestry:
  - Beast
  - Manticore
ev: "72"
stamina: "0350"
speed: 1
movement: Fly
size: "2"
stability: 2
free_strike: 6
might: 4
agility: 3
reason: 0
intuition: 0
presence: -1
traits:
  - name: Solo Monster
    effects:
      - effect: At the end of each of their turns, the manticore can take 10 damage to
          end one effect on them that can be ended by a saving throw. This
          damage can't be reduced in any way.
        name: End Effect
      - effect: The manticore can take two turns each round. They can't take turns
          consecutively.
        name: Solo Turns
  - name: Agile Predator
    effects:
      - effect: Whenever the manticore deals damage to a creature, they don't provoke
          opportunity attacks from that creature during that turn.
abilities:
  - name: Carnivorous Bite
    icon: 🗡
    cost: Signature Ability
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Main action
    distance: Melee 1
    target: One creature or object
    effects:
      - roll: Power Roll + 4
        t1: 12 damage; A < 2 bleeding (save ends)
        t2: 17 damage; A < 3 bleeding (save ends)
        t3: 21 damage; A < 4 bleeding (save ends)
      - effect: If the target is frightened, this ability gains an edge.
        name: Effect
  - name: Tail Spike
    icon: 🏹
    keywords:
      - Ranged
      - Strike
      - Weapon
    type: Main action
    distance: Ranged 10
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        t1: 6 damage; M < 2 4 poison damage
        t2: 11 damage; M < 3 4 poison damage, weakened (save ends)
        t3: 14 damage; M < 4 8 poison damage, weakened (save ends)
      - effect: While weakened this way, a target takes 1d6 poison dam- age at the start
          of each of their turns.
        cost: 1 Malice
  - name: Harrying Claws
    icon: 🗡
    keywords:
      - Melee
      - Strike
      - Weapon
    type: Maneuver
    distance: Melee 1
    target: Two creatures or objects
    effects:
      - cost: ≤11
        effect: Slide 1; A < 2 3 damage
        t2: Slide 2; A < 3 5 damage
        t3: Slide 4; A < 4 7 damage
  - name: Reflexive Instinct
    icon: ❗️
    cost: 2 Malice
    keywords:
      - Ranged
    type: Triggered action
    distance: Ranged 10
    target: The triggering creature
    trigger: A creature within distance deals damage to the manticore.
    effects:
      - effect: The manticore shifts up to 5 squares into the air, then can use Tail
          Spike against the target.
        name: Effect
  - name: Trumpeting Howl
    icon: ☠️
    cost: Villain Action 1
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 5 burst
    target: Each creature in the area
    effects:
      - cost: ≤11
        effect: Frightened (EoT); if the target has I < 2 they are instead frightened
          (save ends)
        t2: Frightened (EoT); if the target has I < 3 they are instead frightened (save
          ends)
        t3: Frightened (EoT); if the target has I < 4 they are instead dazed (save ends)
  - name: Cornered Predator
    icon: ☠️
    cost: Villain Action 2
    keywords:
      - "-"
    type: "-"
    distance: Self
    target: Self
    effects:
      - effect: The manticore shifts up to their speed, then can use Tail Spike against
          each enemy within distance of that ability.
        name: Effect
  - name: Debilitating Poison
    icon: ☠️
    cost: Villain Action 3
    keywords:
      - "-"
    type: "-"
    distance: Self
    target: Self
    effects:
      - effect: The manticore sours their poison with enmity. Until the end of the
          encounter, the manticore has a double edge on power rolls against
          weakened creatures. Additionally, any creature weakened by the
          manticore's Tail Spike ability has their speed halved and takes an
          extra 3 poison damage at the start of each of their turns.
        name: Effect
~~~