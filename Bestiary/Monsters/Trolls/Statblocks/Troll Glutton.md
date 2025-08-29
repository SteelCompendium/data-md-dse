---
agility: 1
ancestry:
- Giant
- Troll
ev: '28'
file_basename: Troll Glutton
file_dpath: Monsters/Trolls/Statblocks
free_strike: 7
intuition: 0
item_id: troll-glutton
item_index: '411'
item_name: Troll Glutton
level: 5
might: 3
presence: 1
reason: -1
roles:
- Elite Brute
scc:
- mcdm.monsters.v1:monster:troll-glutton
scdc:
- 1.1.1:2:411
size: '2'
source: mcdm.monsters.v1
speed: 6
stability: 4
stamina: '160'
type: monster
---

~~~ds-statblock
name: Troll Glutton
level: 5
roles:
  - Elite Brute
ancestry:
  - Giant
  - Troll
ev: "28"
stamina: "160"
weaknesses:
  - Acid 5
  - fire
speed: 6
size: "2"
stability: 4
free_strike: 7
might: 3
agility: 1
reason: -1
intuition: 0
presence: 1
traits:
  - name: Insatiable Appetite
    effects:
      - effect: Once per turn, the glutton can use the Charge main actionas a free
          maneuver if they target a winded creature.
  - name: Relentless Hunger
    effects:
      - effect: The glutton dies only if they are reduced to 0 Stamina by acid or fire
          damage, if they end their turn with 0 Stamina, or if they take acid or
          fire damage while at 0 Stamina
abilities:
  - name: Voracious Mastication
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
      - roll: Power Roll + 3
        t1: 10 damage
        t2: 15 damage; M < 2 slowed (save ends)
        t3: 18 damage; M < 3 slowed (save ends)
      - effect: The glutton regains Stamina equal to the damage dealt.
        cost: 1 Malice
  - name: Crash Through
    icon: 👤
    cost: 3 Malice
    keywords:
      - "-"
    type: Main action
    distance: Self
    target: Self
    effects:
      - effect: The glutton shifts up to their speed in a straight line, ignoring
          difficult terrain. The first time during this movement that the
          glutton moves through the space of a creature or object their size or
          smaller, that creature or object takes 10 damage, or a creature can
          choose to fall prone instead. If the glutton moves into a creature or
          object larger than them and doesn't knock the creature prone or
          destroy the object, the glutton's movement ends and they are dazed
          until the end of their next turn.
        name: Effect
  - name: Food Frenzy
    icon: 👤
    keywords:
      - "-"
    type: Maneuver
    distance: Self
    target: Self
    effects:
      - effect: Until the start of their next turn, the glutton has a double edge on
          strikes, and strikes made against them gain an edge
        name: Effect
  - name: Spiteful Retort
    icon: ❗️
    cost: 1 Malice
    keywords:
      - Melee
    type: Free triggered action
    distance: Melee 1
    target: The triggering creature
    trigger: The glutton is reduced to 0 Stamina but doesn't die.
    effects:
      - effect: The glutton uses Voracious Mastication against an adjacent creature.
        name: Effect
~~~