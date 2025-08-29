---
agility: 4
ancestry:
- Dragon
- Elemental
ev: '72'
file_basename: Gloom Dragon
file_dpath: Monsters/Dragons/Statblocks
free_strike: 6
intuition: 3
item_id: gloom-dragon
item_index: '344'
item_name: Gloom Dragon
level: 4
might: 2
presence: 4
reason: 1
roles:
- Solo
scc:
- mcdm.monsters.v1:monster:gloom-dragon
scdc:
- 1.1.1:2:344
size: '4'
source: mcdm.monsters.v1
speed: 8
stability: 2
stamina: '350'
type: monster
---

~~~ds-statblock
name: Gloom Dragon
level: 4
roles:
  - Solo
ancestry:
  - Dragon
  - Elemental
ev: "72"
stamina: "350"
immunities:
  - Psychic 5
speed: 8
movement: Fly, hover
size: "4"
stability: 2
free_strike: 6
might: 2
agility: 4
reason: 1
intuition: 3
presence: 4
traits:
  - name: Solo Monster
    effects:
      - effect: At the end of each of their turns, the dragon can take 10 damage to end
          one effect on them that can be ended by a saving throw. This damage
          can't be reduced in any way.
        name: End Effect
      - effect: The dragon can take two turns each round. They can't take turns
          consecutively.
        name: Solo Turns
  - name: Gloaming Wyrmscale Aura
    effects:
      - effect: The dragon's scales create a 3 aura of dark supernatural fog around them
          that feeds on their victims' fears and provides concealment to the
          dragon only. Each enemy who starts their turn in the area takes 2
          psychic damage. Additionally, whenever one or more enemies is in the
          area, the dragon's abilities deal an extra 3 psychic damage.
  - name: Shadow Skulk
    effects:
      - effect: Once per turn, the dragon can shift up to their speed, leaving behind a
          4 cube area of magical darkness in their starting space that lasts
          until the end of the encounter. The dragon ignores concealment created
          by this darkness. Any enemy who ends their turn in the area and has I
          < 3 is frightened of the dragon until the end of their next turn.
  - name: Dread and Terror
    effects:
      - effect: The dragon thickens the fog of their Gloaming Wyrmscale Aura trait and
          the horrors within it. Each creature in the area takes a bane on
          strikes made against the dragon until the start of the dragon's next
          turn.
  - name: Doleful Visions
    effects:
      - effect: The dragon manifests four 2 cubes of nightmarish apparitions anywhere on
          the encounter map. Each creature in the area when it appears makes an
          **Intuition test**.
        t1: 14 damage; dazed (save ends)
        t2: 11 damage; dazed (EoT)
        t3: 6 damage
  - name: Solo Action
    effects:
      - effect: The dragon takes an additional main action on their turn. They can use
          this feature even if they are dazed.
  - name: Phantasmagoria!
    effects:
      - effect: The dragon summons macabre, disquieting phantasms in a 10 cube within 1
          square that lasts until the end of the encounter. Any enemy who enters
          the area for the first time in a round or starts their turn there
          takes 6 psychic damage, or 8 psychic damage if they are dragonsealed
          by the gloom dragon. Additionally, the enemy's Intuition score is
          treated as 1 lower for the purpose of resisting potencies until the
          end of the encounter.
abilities:
  - name: Breath of Brume
    icon: 🔳
    cost: Signature Ability
    keywords:
      - Area
      - Magic
      - Ranged
    type: Main action
    distance: 4 cube within 10
    target: Each enemy and object in the area
    effects:
      - name: Effect
        effect: Each target makes an **Agility test**.
        t1: 14 cold damage; the target is dragonsealed (save ends)
        t2: 11 cold damage; the target is dragonsealed (save ends)
        t3: 6 cold damage
      - effect: A dragonsealed creature has psychic weakness 3 and cold weakness 3.
          Additionally, the area is filled with magical darkness. The dragon
          ignores concealment created by this darkness.
  - name: Phantom Tail Swing
    icon: 🗡
    keywords:
      - Charge
      - Magic
      - Melee
      - Strike
    type: Main action
    distance: Melee 3
    target: Two creatures or objects
    effects:
      - roll: Power Roll + 4
        t1: 10 psychic damage; pull 2
        t2: 15 psychic damage; pull 4
        t3: 18 psychic damage; pull 6
      - effect: The pull becomes a vertical slide.
        cost: 3 Malice
  - name: Visions in the Dark
    icon: ❇️
    cost: 5 Malice
    keywords:
      - Area
      - Magic
    type: Maneuver
    distance: 10 burst
    target: Each enemy in the area
    effects:
      - effect: Each target must be dragonsealed. Each target takes 3 psychic damage,
          and if they have I < 3 they immediately make a free strike against one
          ally of the dragon's choice.
        name: Effect
  - name: Encroaching Darkness
    icon: ❗️
    cost: 1 Malice
    keywords:
      - "-"
    type: Free triggered action
    distance: Self
    target: Self
    trigger: A creature within 10 squares moves.
    effects:
      - effect: The dragon moves two existing cubes of magical darkness they created up
          to 10 squares each.
        name: Effect
  - name: Enveloping Umbrage
    icon: ☠️
    cost: Villain Action 1
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 5 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        t1: Pull 2; I < 2 frightened (EoT)
        t2: Pull 4; I < 3 frightened (save ends)
        t3: Pull 6; I < 4 frightened (save ends)
  - name: Pall of Nightmares
    icon: ☠️
    cost: Villain Action 2
    keywords:
      - Area
      - Magic
    type: "-"
    distance: 10 burst
    target: Each enemy in the area
    effects:
      - roll: Power Roll + 4
        t1: 6 psychic damage
        t2: 11 psychic damage
        t3: 14 psychic damage
      - effect: Each target must be dragonsealed. Any target who has I < 3 is also dazed
          (save ends).
        name: Effect
  - name: Absence of All Light
    icon: ☠️
    cost: Villain Action 3
    keywords:
      - "-"
    type: "-"
    distance: Special
    target: Special
    effects:
      - effect: The dragon disappears from the encounter map. The dragon and three
          hallucinatory illusions of themself then immediately reappear in
          unoccupied spaces on the encounter map, and the dragon and each
          illusion uses Breath of Brume. Each illusion is indistinguishable from
          the dragon except by supernatural means, has 1 Stamina, and has the
          dragon's speed. An illusion acts on the dragon's turns but can take
          only move actions. Once per round before or after using an ability,
          the dragon can trade places with any duplicate.
        name: Effect
~~~